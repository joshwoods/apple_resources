

- App Store Connect API
-  Create recruitment criteria 

Web Service Endpoint

# Create recruitment criteria

Create new criteria for recruiting testers for your TestFlight build.

App Store Connect API 3.8+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/betaRecruitmentCriteria
```

## HTTP Body

BetaRecruitmentCriterionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BetaRecruitmentCriterionResponse

`Created`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Resending Invitations

Modify recruitment criteria

Update the recruitment criteria for your TestFlight build.

Remove recruitment criteria 

Remove the recruitment criteria for your TestFlight build.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

Read recruitment criteria options

Get a list of the possible beta recruitment criteria options.

