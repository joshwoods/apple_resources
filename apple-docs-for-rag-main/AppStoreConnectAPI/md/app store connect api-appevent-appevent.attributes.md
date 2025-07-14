

- App Store Connect API
- AppEvent
-  AppEvent.Attributes 

Object

# AppEvent.Attributes

The attributes that describe an In-App event.

App Store Connect API 1.7+

``` source
object AppEvent.Attributes
```

## Properties

`archivedTerritorySchedules`

`[`AppEvent.Attributes.ArchivedTerritorySchedules`]`

`badge`

`string`

Possible Values: `LIVE_EVENT, PREMIERE, CHALLENGE, COMPETITION, NEW_SEASON, MAJOR_UPDATE, SPECIAL_EVENT`

`deepLink`

`uri`

`eventState`

`string`

Possible Values: `DRAFT, READY_FOR_REVIEW, WAITING_FOR_REVIEW, IN_REVIEW, REJECTED, ACCEPTED, APPROVED, PUBLISHED, PAST, ARCHIVED`

`primaryLocale`

`string`

`priority`

`string`

Possible Values: `HIGH, NORMAL`

`purchaseRequirement`

`string`

Possible values: `NO_COST_ASSOCIATED`, `IN_APP_PURCHASE`

`purpose`

`string`

Possible Values: `APPROPRIATE_FOR_ALL_USERS, ATTRACT_NEW_USERS, KEEP_ACTIVE_USERS_INFORMED, BRING_BACK_LAPSED_USERS`

`referenceName`

`string`

`territorySchedules`

`[`AppEvent.Attributes.TerritorySchedules`]`

## Mentioned in 

App Store Connect API 3.6 release notes

## Topics

### Objects

object AppEvent.Attributes.ArchivedTerritorySchedules

object AppEvent.Attributes.TerritorySchedules

## See Also

### Objects

object AppEvent.Relationships

