

- App Store Connect API
-  Read age rating declaration 

Web Service Endpoint

# Read age rating declaration

Get the age rating declaration for the app info.

App Store Connect API 1.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appInfos/{id}/ageRatingDeclaration
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Infos resource.

## Query Parameters

`fields[ageRatingDeclarations]`

`[string]`

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

## Response Codes

` 200 ``OK`

AgeRatingDeclarationResponse

`OK`

The request completed successfully.

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

## Discussion

Responses for this endpoint include the `gamblingAndContests` attribute for legacy clients. For new clients, use `contents` or `gambling` properties instead. For example, in an app that has a `FREQUENT_OR_INTENSE` declaration for contests, the age rating for the `AppInfos` is 12+. If you declare a value of true for `gamblingAndContests` instead, the age rating for the `AppInfos` is 17+.

Important

The `gamblingAndContests` property is deprecated. Use the `contests` or `gambling` properties instead.

### Read the Age Rating Declaration

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/appInfos/994af4c0-ff6c-fdb9-e053-d23ab111187e/ageRatingDeclaration
```

```
{
  "data": {
    "type": "ageRatingDeclarations",
    "id": "994af4c0-ff6c-fdb9-e053-d23ab111187e",
    "attributes": {
      "alcoholTobaccoOrDrugUseOrReferences": "NONE",
      "contests": "FREQUENT_OR_INTENSE",
      "gamblingAndContests": true,
      "gambling": false,
      "gamblingSimulated": "NONE",
      "kidsAgeBand": null,
      "medicalOrTreatmentInformation": "NONE",
      "profanityOrCrudeHumor": "NONE",
      "sexualContentGraphicAndNudity": "NONE",
      "sexualContentOrNudity": "NONE",
      "seventeenPlus": false,
      "horrorOrFearThemes": "NONE",
      "matureOrSuggestiveThemes": "NONE",
      "unrestrictedWebAccess": false,
      "violenceCartoonOrFantasy": "NONE",
      "violenceRealisticProlongedGraphicOrSadistic": "NONE",
      "violenceRealistic": "NONE"
    },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/994af4c0-ff6c-fdb9-e053-d23ab111187e"
  }
},
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/appInfos/994af4c0-ff6c-fdb9-e053-d23ab111187e/ageRatingDeclaration"
  }
}
```

