# Documenting API headers

This file documents the header parameters for a fictional application called Phantastic Foto. 

## Header query parameters

The following header query parameters are for a request to upload a photo.

| Header name | Description | Required | Values |
| ----        | ----        | ----     | ----   |
| Content-Type | The format of the photo to upload. | Optional | Valid values are: image/jpg, image/png, image/gif. Default is image/jpg. |
| Accept | The format for the data to return. | Optional | Valid values are: application/json, application/xml. Default is application/json. |

### Sample request

This request uploads a photo in JPG and returns data in XML.

POST `https://phantasticFoto/api/v1/photo`

Content-Type: image/jpg <br>
Accept: application/xml

POST body is the image to upload. 
