

- App Store Connect API
- AppStoreVersionUpdateRequest
- AppStoreVersionUpdateRequest.Data
-  AppStoreVersionUpdateRequest.Data.Attributes 

Object

# AppStoreVersionUpdateRequest.Data.Attributes

Attributes whose values you’re changing as part of the update request.

App Store Connect API 1.2+

``` source
object AppStoreVersionUpdateRequest.Data.Attributes
```

## Properties

`copyright`

`string`

`earliestReleaseDate`

`date-time`

`releaseType`

`string`

Possible Values: `MANUAL, AFTER_APPROVAL, SCHEDULED`

`versionString`

`string`

`downloadable`

`boolean`

`reviewType`

`string`

`NOTARIZATION` is alternative app marketplace distribution. All eligible app versions default to both `APP_STORE` and `NOTARIZATION.` An app can be distributed on either or both.

Possible Values: `APP_STORE, NOTARIZATION`

## Mentioned in 

Configuring alternative marketplaces and alternative marketplace apps

## See Also

### Objects

object AppStoreVersionUpdateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

