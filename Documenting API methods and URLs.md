# Documenting API methods and URLs

This file documents API methods and URLs for a fictional application called Phantastic Foto.

# About Phanstastic Foto API

The Phantastic Photo API allows users to share and print photos. The API is based on REST principles and accesses data using HTTP protocol. 

# Requests

The requests available for the Phantastic Foto API are described as follows.

## Create an album

Creates a collection of images.

POST `https://phantasticfoto.com/api/v1`

## Retreive an album

Returns data about a collection of images.

GET `https://phantasticfoto.com/api/v1/album/{album ID}`

where {album ID} is the ID of the album to retreive.

## Update an album

Makes changes to an existing collection of images. 

PUT `https://phantasticfoto.com/api/v1/album/{album ID}`

where {album ID]} is the ID of the album to update.

## Delete an album

Deletes an existing collection of images.

DELETE `https://phantasticfoto.com/api/v1/album/{album ID}`

where {album ID} is the ID of the album to delete.

## View all albums

Returns a list of all of the user's albums.

GET `https://phantasticfoto.com/api/v1/album`

## Print an album

Prints a collection of images. 

POST `https://phantasticfoto.com/api/v1/album/{album ID}/print`

where {album ID} is the ID of the album to print.
