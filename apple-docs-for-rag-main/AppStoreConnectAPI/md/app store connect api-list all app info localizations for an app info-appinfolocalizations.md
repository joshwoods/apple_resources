

- App Store Connect API
-  List All App Info Localizations for an App Info 

Web Service Endpoint

# List All App Info Localizations for an App Info

Get a list of localized, app-level information for an app.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appInfos/{id}/appInfoLocalizations
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[appInfoLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `locale, name, subtitle, privacyPolicyUrl, privacyChoicesUrl, privacyPolicyText, appInfo`

`fields[appInfos]`

`[string]`

Fields to return for included related types.

Possible Values: `appStoreState, state, appStoreAgeRating, australiaAgeRating, brazilAgeRating, brazilAgeRatingV2, franceAgeRating, koreaAgeRating, kidsAgeBand, app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`filter[locale]`

`[string]`

Fields to return for included related types.

`include`

`[string]`

Relationship data to include in the response.

Value: `appInfo`

`limit`

`integer`

Number of included related resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

AppInfoLocalizationsResponse

`OK`

Request succeeded.

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Reading App Localization Information

Read App Info Localization Information

Read localized app-level information.

