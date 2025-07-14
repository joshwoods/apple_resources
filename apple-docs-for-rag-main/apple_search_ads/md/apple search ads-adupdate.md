

- Apple Search Ads
-  AdUpdate 

Object

# AdUpdate

The request to update an ad.

Search Ads 4.0+

``` source
object AdUpdate
```

## Properties

`creativeId`

`int64`

 (Read-only) 

The unique identifier for a creative.

`adGroupId`

`int64`

 (Read-only) 

The unique identifier for an AdGroup.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ads.

`campaignId`

`int64`

 (Read-only) 

The unique identifier for a campaign.

`creationTime`

`date-time`

 (Read-only) 

The date and time of the creation of the `AdUpdate` object.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` Selector Condition operators with Find Ads.

`creativeType`

`string`

 (Read-only) 

The type of creative.

See CreativeType for value descriptions.

You can create one Creative per custom product page per organization.

You can use the `EQUALS` Selector Condition operator with Find Ads.

`deleted`

`boolean`

 (Read-only) 

Indicates whether an Ad is deleted.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ads.

Default: `false`

`id`

`int64`

 (Read-only) 

An `adId` is a unique identifier that represents the assignment relationship between an ad group and an ad.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ads.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the Ad.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` Selector Condition operators with Find Ads.

`name`

`string`

The unique name of the Ad assigned to an AdGroup.

This field is required in requests and is updatable.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` Selector Condition operators with Find Ads.

Maximum length: `255`

`orgId`

`int64`

 (Read-only) 

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`servingStateReasons`

`[string]`

 (Read-only) 

A list of reasons that displays when an Ad isn’t running. For example, if the DeviceClass changes, the `servingStateReasons` may change.

See AdServingStateReasons for value descriptions.

`servingStatus`

`string`

 (Read-only) 

The indicator of the status of an ad assignment with an AdGroup.

See AdServingStatus for value descriptions.

`status`

`string`

The status of the Ad.

This field is required in requests and is updatable.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ads.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## See Also

### Ad Request and Response Objects

object Ad

The assignment of a creative to an ad group.

object AdCreate

The request to create an ad, and assign a creative to an ad group.

object AdResponse

The response to an ad request.

object AdListResponse

The response to a request that returns a list of ads.

