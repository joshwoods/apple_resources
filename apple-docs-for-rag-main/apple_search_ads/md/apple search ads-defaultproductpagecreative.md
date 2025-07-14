

- Apple Search Ads
-  DefaultProductPageCreative 

Object

# DefaultProductPageCreative

The default product page object.

``` source
object DefaultProductPageCreative
```

## Properties

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier.

`creationTime`

`date-time`

 (Read-only) 

The timestamp for the creation of the report in the format of `YYYY-MM-DD’T’HH:mm:ss.SSS`.

`id`

`int64`

 (Read-only) 

The unique identifier for a creative.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

`name`

`string`

 (Required) 

The unique name of the creative.

Minimum length: `1`

Maximum length: `200`

`orgId`

`int64`

 (Read-only) 

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`productPageId`

`string`

The product page identifier.

`state`

`string`

 (Read-only) 

The system state of the process.

`stateReasons`

`[string]`

 (Read-only) 

A list of reasons that displays when an ad isn’t running.

`type`

`string`

 (Required) 

The type of creative.

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

object CustomProductPageCreative

The creative details of a product page.

object CreativeResponse

The response details of a creative request.

object CreativeListResponse

A container for response details of a creative request.

object MediaAppAsset

The asset details of app preview or app screenshots.

object MediaAppAssetsDetail

The app asset details of a device.

