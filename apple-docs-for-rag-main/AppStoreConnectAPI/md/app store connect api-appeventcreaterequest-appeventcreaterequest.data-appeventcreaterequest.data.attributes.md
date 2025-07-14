

- App Store Connect API
- AppEventCreateRequest
- AppEventCreateRequest.Data
-  AppEventCreateRequest.Data.Attributes 

Object

# AppEventCreateRequest.Data.Attributes

App Store Connect API 1.7+

``` source
object AppEventCreateRequest.Data.Attributes
```

## Properties

`badge`

`string`

Possible Values: `LIVE_EVENT, PREMIERE, CHALLENGE, COMPETITION, NEW_SEASON, MAJOR_UPDATE, SPECIAL_EVENT`

`deepLink`

`uri`

`primaryLocale`

`string`

`priority`

`string`

Possible Values: `HIGH, NORMAL`

`purchaseRequirement`

`string`

`purpose`

`string`

Possible Values: `APPROPRIATE_FOR_ALL_USERS, ATTRACT_NEW_USERS, KEEP_ACTIVE_USERS_INFORMED, BRING_BACK_LAPSED_USERS`

`referenceName`

`string`

 (Required) 

`territorySchedules`

`[`AppEventCreateRequest.Data.Attributes.TerritorySchedules`]`

## Topics

### Objects

object AppEventCreateRequest.Data.Attributes.TerritorySchedules

## See Also

### Objects

object AppEventCreateRequest.Data.Relationships

