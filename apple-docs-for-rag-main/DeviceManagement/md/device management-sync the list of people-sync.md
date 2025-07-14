

- Device Management
-  Sync the List of People 

Web Service Endpoint

# Sync the List of People

Get updates about the list of people the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/person/sync
```

## HTTP Body

RosterRequest

The object containing the request information.

Content-Type: application/json

## Response Codes

` 200 ``OK`

RosterPersonResponse

`OK`

The request was successful. The server returns a list of people.

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

The server was unable to process the request.

## Discussion

This sync service uses a cursor returned by the full person-roster service. It returns a list of all modifications (additions or deletions) made since the cursor date, for up to 7 days.

This service may return the same person more than once. You can identify duplicates by matching their `unique_identifier` values.

## See Also

### People Management

object RosterPerson

A person’s properties and their values.

Get the List of People

Obtain a list of people the server manages, across the organization.

