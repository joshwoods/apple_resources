

- Device Management
-  Get the List of People 

Web Service Endpoint

# Get the List of People

Obtain a list of people the server manages, across the organization.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/roster/class/person
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

In addition to instructors and students, this list may contain additional people who don’t belong to any class.

## Topics

### Response

object RosterPersonResponse

The response that contains the people in the organization.

## See Also

### People Management

object RosterPerson

A person’s properties and their values.

Sync the List of People

Get updates about the list of people the server manages.

