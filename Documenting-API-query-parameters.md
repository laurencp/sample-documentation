# Documenting API query parameters

This file documents API query parameters for a fictional company called BugSquisher. BugSquisher makes bug tracking software.

## About the BugSquisher API

The BugSquisher API enables users to create and manage bugs for quality assurance.

## Query parameters

The following query parameters are for a request to return a list of bugs. You can choose which bugs will be returned by using the query parameters. 

| Parameter | Description | Type | Required | Notes |
| ----      | ----        | ---- | ----     | ----  |
| startDate | The start date for when the bug was created. | Date | Optional | Format is YYYY-MM-DD. The default is the earliest recorded bug. |
| endDate   | The end date for when the bug was created. | Date | Optional | Format is YYYY-MM-DD. The default is today's date. |
| priority  | How important the bug is. | Integer | Optional | Value returned is an integer of 1 to 4, where 1 is the highest priority. The default is all priorities. |
| severity  | How big the impact is. | Integer | Optional | Value returned is an integer of 1 to 4, where 1 is the most severe. The default is all severities. |
| status    | The status of the bug. | String | Optional | Valid values are: open, closed, duplicate, notabug. Default is all statuses. |
| start     | The starting index of bugs to return. | Integer | Optional | Zero is the first bug on the list. The default is zero. |
| total     | The total number of bugs to return. | Integer | Optional | The default is the total number of bugs minus the start value. |

### Sample request

This request returns the first 20 open bugs in the year 2015 where the priority and severity are both 1.

GET `https://api.bugsquisher.com/bug?startDate=2015-01-01&endDate=2015-12-31&priority=1&severity=1&status=open&start=0&total=20` 
