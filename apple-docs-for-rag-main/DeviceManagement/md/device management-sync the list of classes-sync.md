

- Device Management
-  Sync the List of Classes 

Web Service Endpoint

# Sync the List of Classes

Get updates about the list of classes the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/sync
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

## Discussion

This sync service uses a cursor that is returned by the full class-roster service. It returns a list of all modifications (additions or deletions) made since the cursor date, for up to 7 days.

This service may return the same class more than once. You can identify duplicates by matching their `unique_identifier` values.

## See Also

### Class Management

object RosterClass

A class’s properties and their values.

Get the List of Classes

Obtain a list of classes the server manages.

