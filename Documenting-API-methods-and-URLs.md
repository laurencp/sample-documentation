# Documenting API methods and URLs

This file documents API methods and URLs for a fictional application called Phantastic Foto.

## About Phanstastic Foto API

The Phantastic Photo API allows users to share and print photos. 

The API is based on REST principles and accesses data using HTTP protocol. 

## Requests

The requests available for the Phantastic Foto API are:
1. [Create an album](#create)
2. [Update an album](#update)
3. [Delete an album](#delete)
4. [Retreive an album](#retreive)
5. [Retreive a list of all albums](#view-all)
6. [Print an album](#print)

### Create an album <a name="create"></a>

Creates a collection of images.

POST `https://phantasticfoto.com/api/v1`

### Update an album <a name="update"></a>

Makes changes to an existing collection of images. 

PUT `https://phantasticfoto.com/api/v1/album/{album ID}`

where {album ID]} is the ID of the album to update.

### Delete an album <a name="delete"></a>

Deletes an existing collection of images.

DELETE `https://phantasticfoto.com/api/v1/album/{album ID}`

where {album ID} is the ID of the album to delete.

### Retreive an album <a name="retreive"></a>

Returns data about a specific collection of images.

GET `https://phantasticfoto.com/api/v1/album/{album ID}`

where {album ID} is the ID of the album to retreive.

### Retreive a list of all albums <a name="view-all"></a>

Returns a list of all of the user's albums.

GET `https://phantasticfoto.com/api/v1/album`

### Print an album <a name="print"></a>

Prints a collection of images. 

POST `https://phantasticfoto.com/api/v1/album/{album ID}/print`

where {album ID} is the ID of the album to print.
