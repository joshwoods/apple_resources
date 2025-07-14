

- App Store Connect API
-  Read recruitment criteria options 

Web Service Endpoint

# Read recruitment criteria options

Get a list of the possible beta recruitment criteria options.

App Store Connect API 3.8+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaRecruitmentCriterionOptions
```

## Query Parameters

`fields[betaRecruitmentCriterionOptions]`

`[string]`

Value: `deviceFamilyOsVersions`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

BetaRecruitmentCriterionOptionsResponse

`OK`

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

## See Also

### Resending Invitations

Create recruitment criteria

Create new criteria for recruiting testers for your TestFlight build.

Modify recruitment criteria

Update the recruitment criteria for your TestFlight build.

Remove recruitment criteria 

Remove the recruitment criteria for your TestFlight build.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

