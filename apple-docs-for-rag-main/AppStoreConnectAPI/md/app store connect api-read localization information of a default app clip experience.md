

- App Store Connect API
-  Read Localization Information of a Default App Clip Experience 

Web Service Endpoint

# Read Localization Information of a Default App Clip Experience

Get localized metadata that appears on the App Clip card of a specific default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipDefaultExperienceLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Default App Clip Experience Localizations resource.

## Query Parameters

`fields[appClipDefaultExperienceLocalizations]`

`[string]`

Additional fields to include for each Default App Clip Experience Localizations resource returned by the response.

Possible Values: `locale, subtitle, appClipDefaultExperience, appClipHeaderImage`

`fields[appClipHeaderImages]`

`[string]`

Additional fields to include for each Default App Clip Experience Localizations resource returned by the response.

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, uploadOperations, assetDeliveryState, appClipDefaultExperienceLocalization`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `appClipDefaultExperience, appClipHeaderImage`

## Response Codes

` 200 ``OK`

AppClipDefaultExperienceLocalizationResponse

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

## See Also

### Getting Metadata for Your Default App Clip Experience

Read App Clip Card Image Information for a Localized Default App Clip Experience

Get the image that appears on the App Clip card, specific to a locale, for a default App Clip experience.

