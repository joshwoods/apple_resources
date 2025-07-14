

- App Store Connect API
-  Read the Age Rating Declaration Information of an App Store Version Deprecated

Web Service Endpoint

# Read the Age Rating Declaration Information of an App Store Version

Get the age-related information declared for your app.

App Store Connect API 1.2–1.4Deprecated

Deprecated

Use Read age rating declaration instead.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/ageRatingDeclaration
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[ageRatingDeclarations]`

`[string]`

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

## Response Codes

` 200 ``OK`

AgeRatingDeclarationWithoutIncludesResponse

`OK`

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

App Store Connect API 1.3 release notes

## See Also

### Reading Declarations

Read the Routing App Coverage Information of an App Store Version

Get the routing app coverage file that is associated with a specific App Store version

