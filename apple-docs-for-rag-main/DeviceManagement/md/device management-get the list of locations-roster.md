

- Device Management
-  Get the List of Locations 

Web Service Endpoint

# Get the List of Locations

Obtain a list of the locations the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/location
```

## HTTP Body

RosterRequest

The object containing the request information.

Content-Type: application/json

## Response Codes

` 200 ``OK`

RosterClassLocationResponse

`OK`

The request was successful. The server returns a list of locations.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server was unable to process the request.

## Topics

### Response

object RosterClassLocationResponse

The response that contains a list of locations.

## See Also

### Location Mangement

object BaseRosterLocation

A base location’s properties and their values.

object RosterLocation

A location’s properties and their values.

Sync the Locations

Get updates about the list of locations the server manages.

