

- Apple Search Ads
-  CustomProductPageCreative 

Object

# CustomProductPageCreative

The creative details of a product page.

Search Ads 4.0+

``` source
object CustomProductPageCreative
```

## Properties

`productPageId`

`string`

 (Required) 

A unique string to identify a product page on App Store Connect, such as `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier. You can obtain your `adamId` through Get a Campaign or Get all Campaigns.

`creationTime`

`date-time`

 (Read-only) 

The date and time of the creation of the Creative object.

`id`

`int64`

 (Read-only) 

The `creativeId` is a unique identifier for a creative.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

`name`

`string`

 (Required) 

The name of a creative.

Minimum length: `1`

Maximum length: `200`

`orgId`

`int64`

 (Read-only) 

The identifier of the organization that owns a campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`state`

`string`

 (Read-only) 

The system state of the custom product page that indicates whether the page is visible.

See CreativeState for value descriptions.

`stateReasons`

`[string]`

 (Read-only) 

The detailed explanation of the system state.

See CreativeStateReason for value descriptions.

`type`

`string`

 (Required) 

The type of creative.

See CreativeType for value descriptions.

## See Also

### Creative Request and Response Objects

object AppPreviewDevicesMappingResponse

The app preview device mapping response to display name and size mapping requests.

object Creative

The creative object.

object CreativeLocalization

The localized creative metadata.

object CreativeLocalizationWithAssets

The localized creative metadata with app preview.

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

