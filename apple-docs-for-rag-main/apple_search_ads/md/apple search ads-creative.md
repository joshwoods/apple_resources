

- Apple Search Ads
-  Creative 

Object

# Creative

The creative object.

Search Ads 4.0+

``` source
object Creative
```

## Properties

`adamId`

`int64`

Your unique App Store app identifier. Use Get a Campaign or Get all Campaigns to obtain your `adamId`.

This field is required in requests to Create a Creative.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Creatives.

`creationTime`

`date-time`

 (Read-only) 

The date and time of the creation of the Creative object.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` Selector Condition operators with Find Creatives.

`id`

`int64`

 (Read-only) 

The `creativeId` is a unique identifier for a creative.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Creatives.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` Selector Condition operators with Find Creatives.

`name`

`string`

The name of a creative.

This field is required in requests to Create a Creative.

You can use the `EQUALS` and `CONTAINS` Selector Condition operators with Find Creatives.

Minimum length: `1`

Maximum length: `200`

`orgId`

`int64`

 (Read-only) 

The identifier of the organization that owns a campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`state`

`string`

 (Read-only) 

The system state of the creative.

See CreativeState for value descriptions.

`stateReasons`

`[string]`

 (Read-only) 

The detailed explanation of the system state.

See CreativeStateReason for value descriptions.

`type`

`string`

The type of creative.

This field is required in requests to Create a Creative.

See CreativeType for value descriptions.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Creatives.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## See Also

### Creative Request and Response Objects

object AppPreviewDevicesMappingResponse

The app preview device mapping response to display name and size mapping requests.

object CreativeLocalization

The localized creative metadata.

object CreativeLocalizationWithAssets

The localized creative metadata with app preview.

object CustomProductPageCreative

The creative details of a product page.

object CreativeResponse

The response details of a creative request.

object CreativeListResponse

A container for response details of a creative request.

object DefaultProductPageCreative

The default product page object.

object MediaAppAsset

The asset details of app preview or app screenshots.

object MediaAppAssetsDetail

The app asset details of a device.

