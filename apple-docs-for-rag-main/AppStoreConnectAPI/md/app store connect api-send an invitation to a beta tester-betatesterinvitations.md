

- App Store Connect API
-  Send an Invitation to a Beta Tester 

Web Service Endpoint

# Send an Invitation to a Beta Tester

Send or resend an invitation to a beta tester to test a specified app.

App Store Connect API 1.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaTesterInvitations
```

## HTTP Body

BetaTesterInvitationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaTesterInvitationResponse

`Created`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

