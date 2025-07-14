

- App Store Connect API
- Profile
-  Profile.Attributes 

Object

# Profile.Attributes

Attributes that describe a Profiles resource.

App Store Connect API 1.1+

``` source
object Profile.Attributes
```

## Properties

`name`

`string`

`platform`

BundleIdPlatform

`profileContent`

`string`

`uuid`

`string`

`createdDate`

`date-time`

`profileState`

`string`

Possible Values: `ACTIVE, INVALID`

`profileType`

`string`

Possible Values: `IOS_APP_DEVELOPMENT, IOS_APP_STORE, IOS_APP_ADHOC, IOS_APP_INHOUSE, MAC_APP_DEVELOPMENT, MAC_APP_STORE, MAC_APP_DIRECT, TVOS_APP_DEVELOPMENT, TVOS_APP_STORE, TVOS_APP_ADHOC, TVOS_APP_INHOUSE, MAC_CATALYST_APP_DEVELOPMENT, MAC_CATALYST_APP_STORE, MAC_CATALYST_APP_DIRECT`

`expirationDate`

`date-time`

## See Also

### Objects

object Profile.Relationships

The relationships you included in the request and those on which you can operate.

