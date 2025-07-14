

- Device Management
-  Get the List of Classes 

Web Service Endpoint

# Get the List of Classes

Obtain a list of classes the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class
```

## HTTP Body

RosterRequest

The object containing the request information.

Content-Type: application/json

## Response Codes

` 200 ``OK`

RosterClassResponse

`OK`

The request was successful. The server returns a list of classes.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server was unable to process the request.

## Topics

### Request and Response

object RosterRequest

The request for a list of classes.

object RosterClassResponse

The response that contains a list of classes.

## See Also

### Class Management

object RosterClass

A class’s properties and their values.

Sync the List of Classes

Get updates about the list of classes the server manages.

