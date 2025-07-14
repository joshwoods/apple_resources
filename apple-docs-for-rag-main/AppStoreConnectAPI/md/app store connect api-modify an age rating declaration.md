

- App Store Connect API
-  Modify an Age Rating Declaration 

Web Service Endpoint

# Modify an Age Rating Declaration

Provide age-related information so the App Store can determine the age rating for your app.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## HTTP Body

AgeRatingDeclarationUpdateRequest

The request body you use to update an Age Rating Declaration.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AgeRatingDeclarationResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data isn’t valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

App Store Connect API 3.6 release notes

## Discussion

Every app store version has an age rating declaration. Use this endpoint to edit the declaration and provide app-characteristic information so App Store Connect can determine the appropriate age rating for the app.

Use this endpoint to indicate whether an app is Made for Kids.

When calling this endpoint, only include the attributes that you’re modifying.

Important

The `gamblingAndContests` property is deprecated. Use the `contests` or `gambling` properties instead.

For example, in an app that has a `FREQUENT_OR_INTENSE` declaration for contests, the age rating for the `AppInfos` is 12+. If you declare a value of true for `gamblingAndContests` instead, the age rating for the `AppInfos` is 17+.

### Modify an Age Rating Declaration

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/26b5c300-1814-4b7a-8ec9-5411ecf36305

{
  "data": {
    "type": "ageRatingDeclarations",
    "id": "string",
    "attributes": {
      "alcoholTobaccoOrDrugUseOrReferences": "NONE",
      "contests": "NONE",
      "gambling": true,
      "gamblingSimulated": "NONE",
      "medicalOrTreatmentInformation": "NONE",
      "profanityOrCrudeHumor": "NONE",
      "sexualContentGraphicAndNudity": "NONE",
      "sexualContentOrNudity": "NONE",
      "horrorOrFearThemes": "NONE",
      "matureOrSuggestiveThemes": "NONE",
      "unrestrictedWebAccess": true,
      "violenceCartoonOrFantasy": "NONE",
      "violenceRealisticProlongedGraphicOrSadistic": "NONE",
      "violenceRealistic": "NONE",
      "kidsAgeBand": null
    }
  }
}

```

```
{
  "data": {
    "type": "ageRatingDeclarations",
    "id": "26b5c300-1814-4b7a-8ec9-5411ecf36305",
    "attributes": {
      "alcoholTobaccoOrDrugUseOrReferences": "NONE",
      "contests": "NONE",
      “gamblingAndContests”: true,
      "gambling": true,
      "gamblingSimulated": "NONE",
      "medicalOrTreatmentInformation": "NONE",
      "profanityOrCrudeHumor": "NONE",
      "sexualContentGraphicAndNudity": "NONE",
      "sexualContentOrNudity": "NONE",
      "horrorOrFearThemes": "NONE",
      "matureOrSuggestiveThemes": "NONE",
      "unrestrictedWebAccess": true,
      "violenceCartoonOrFantasy": "NONE",
      "violenceRealisticProlongedGraphicOrSadistic": "NONE",
      "violenceRealistic": "NONE",
      "kidsAgeBand": null
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/26b5c300-1814-4b7a-8ec9-5411ecf36305"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/26b5c300-1814-4b7a-8ec9-5411ecf36305"
  }
}

```

### Mark an App as Made for Kids

- Request
- Response

```
PATCH https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/26b5c300-1814-4b7a-8ec9-5411ecf36305

{
  "data": {
    "type": "ageRatingDeclarations",
    "id": "string",
    "attributes": {
      "kidsAgeBand": "FIVE_AND_UNDER"
    }
  }
}
```

```
{
  "data": {
    "type": "ageRatingDeclarations",
    "id": "26b5c300-1814-4b7a-8ec9-5411ecf36305",
    "attributes": {
      "alcoholTobaccoOrDrugUseOrReferences": "NONE",
      "contests": “NONE”,
      “gamblingAndContests”: false,
      "gambling": false,
      "gamblingSimulated": "NONE",
      "medicalOrTreatmentInformation": "NONE",
      "profanityOrCrudeHumor": "NONE",
      "sexualContentGraphicAndNudity": "NONE",
      "sexualContentOrNudity": "NONE",
      "horrorOrFearThemes": "NONE",
      "matureOrSuggestiveThemes": "NONE",
      "unrestrictedWebAccess": true,
      "violenceCartoonOrFantasy": "NONE",
      "violenceRealisticProlongedGraphicOrSadistic": "NONE",
      "violenceRealistic": "NONE",
      "kidsAgeBand": "FIVE_AND_UNDER"
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/26b5c300-1814-4b7a-8ec9-5411ecf36305"
    }
  },
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/ageRatingDeclarations/26b5c300-1814-4b7a-8ec9-5411ecf36305"
  }
}
```

