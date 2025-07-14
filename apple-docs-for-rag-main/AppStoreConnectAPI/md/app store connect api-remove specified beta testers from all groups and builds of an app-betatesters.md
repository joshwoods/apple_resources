

- App Store Connect API
-  Remove Specified Beta Testers from All Groups and Builds of an App 

Web Service Endpoint

# Remove Specified Beta Testers from All Groups and Builds of an App

Remove one or more beta testers’ access to test any builds of a specific app.

App Store Connect API 1.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/apps/{id}/relationships/betaTesters
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## HTTP Body

AppBetaTestersLinkagesRequest

Content-Type: application/json

## Response Codes

` 202 ``Accepted`

`Accepted`

` 204 ``No Content`

`No Content`

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/apps/1000001234/relationships/betaTesters -d
"{
  "data": [
    {
      "type": "betaTesters",
      "id": "b6318884-4aa6-4586-bf0b-be97cf991817"
    }
  ]
}
"
```

```
204 No Content
```

## See Also

### Getting beta tester information for TestFlight

List All Beta Groups for an App

Get a list of beta groups associated with a specific app.

