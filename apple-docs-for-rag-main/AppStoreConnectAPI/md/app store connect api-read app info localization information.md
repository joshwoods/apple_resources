

- App Store Connect API
-  Read App Info Localization Information 

Web Service Endpoint

# Read App Info Localization Information

Read localized app-level information.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appInfoLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appInfoLocalizations]`

`[string]`

Possible Values: `locale, name, subtitle, privacyPolicyUrl, privacyChoicesUrl, privacyPolicyText, appInfo`

`include`

`[string]`

Value: `appInfo`

## Response Codes

` 200 ``OK`

AppInfoLocalizationResponse

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

## See Also

### Reading App Localization Information

List All App Info Localizations for an App Info

Get a list of localized, app-level information for an app.

