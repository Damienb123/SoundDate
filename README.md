# SoundDate

## Table of Contents

1. [Overview](#Overview)
2. [Security](#Security)
3. [Components](#Components)
    - Security Schemes
6. [Example Usage](#Example-Usage)
    - Uploading a Sound File
    - Retrieving Sound Files
7. [Error Handling](#Error-Handling)
    - Error Response Example
8. [Reference](#Reference)

## Overview

The SoundDate API allows users to upload and retrieve sound files associated with their profiles. This API supports two main functionalities: uploading sound files and retrieving sound file information for a specific user.

## Security

This API uses Bearer Authentication. Include the token in the Authorization header of your requests.

## Components

### Security Schemes
BearerAuth:
    - type: http
    - scheme: bearer

## Example Usage

### Uploading a Sound File
To upload a sound file to a user’s profile, send a POST request to the /profile/sound endpoint with the audio file in the request body and the user's authentication token in the header.

### Retrieving Sound Files
To retrieve a list of sound files for a specific user, send a GET request to /user/{userId}/profile/sound with the user’s ID in the path and the authentication token in the header. Optionally, include the sortOrder query parameter to specify the order of the returned sound files.

## Error Handling

If an error occurs, the API will return an error response with an appropriate HTTP status code and a message detailing the error. Common status codes include 401 (Unauthorized) and 413 (Request Entity too large).

## Reference

please refer to the attached .pdf documentation uploaded on this repository needed understanding of the API documentation.
