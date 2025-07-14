

- Device Management
-  Sync the Locations 

Web Service Endpoint

# Sync the Locations

Get updates about the list of locations the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/location/sync
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

## Discussion

This sync service uses a cursor returned by the full location-roster service. It returns a list of all modifications (additions or deletions) made since the cursor date, up to 7 days.

This service may return the same location more than once. You can identify duplicates by matching their `unique_identifier` values.

## See Also

### Location Mangement

object BaseRosterLocation

A base location’s properties and their values.

object RosterLocation

A location’s properties and their values.

Get the List of Locations

Obtain a list of the locations the server manages.

