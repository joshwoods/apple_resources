

- App Store Connect API
-  Read App Info Information 

Web Service Endpoint

# Read App Info Information

Read App Store information including your App Store state, age ratings, Brazil age rating, and kids’ age band.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appInfos/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[appCategories]`

`[string]`

Fields to return for included related types.

Possible Values: `platforms, subcategories, parent`

`fields[appInfoLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `locale, name, subtitle, privacyPolicyUrl, privacyChoicesUrl, privacyPolicyText, appInfo`

`fields[appInfos]`

`[string]`

Fields to return for included related types.

Possible Values: `appStoreState, state, appStoreAgeRating, australiaAgeRating, brazilAgeRating, brazilAgeRatingV2, franceAgeRating, koreaAgeRating, kidsAgeBand, app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`limit[appInfoLocalizations]`

`integer`

Number of included related resources to return.

Maximum: `50`

`fields[ageRatingDeclarations]`

`[string]`

Fields to return for included related types.

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

## Response Codes

` 200 ``OK`

AppInfoResponse

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

## Mentioned in 

App Store Connect API 3.6 release notes

App Store Connect API 3.7 release notes

## Discussion

For request and response examples for reading an age rating declaration, see Read age rating declaration.

## See Also

### Reading App Information

List All App Infos for an App

Get information about an app that is currently live on App Store, or that goes live with the next version.

List All App Info Localizations for an App Info

Get a list of localized, app-level information for an app.

