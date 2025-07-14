

- App Store Connect API
- AppStoreVersion
-  AppStoreVersion.Attributes 

Object

# AppStoreVersion.Attributes

Attributes that describe an App Store Versions resource.

App Store Connect API 1.2+

``` source
object AppStoreVersion.Attributes
```

## Properties

`platform`

Platform

`appStoreState`

AppStoreVersionState

This attribute is deprecated. Use AppVersionState instead.

`copyright`

`string`

`earliestReleaseDate`

`date-time`

`releaseType`

`string`

Possible Values: `MANUAL, AFTER_APPROVAL, SCHEDULED`

`versionString`

`string`

`createdDate`

`date-time`

`downloadable`

`boolean`

`appVersionState`

AppVersionState

`reviewType`

`string`

Possible Values: `APP_STORE, NOTARIZATION`

## Mentioned in 

App Store Connect API 3.3 release notes

App Store Connect API 3.7 release notes

## See Also

### Objects

object AppStoreVersion.Relationships

The relationships you included in the request and those on which you can operate.

