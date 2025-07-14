

- Apple Search Ads
-  CreativeLocalizationWithAssets 

Object

# CreativeLocalizationWithAssets

The localized creative metadata with app preview.

Search Ads 4.0+

``` source
object CreativeLocalizationWithAssets
```

## Properties

`appName`

`string`

The app name on App Store Connect.

`appPreviewDeviceWithAssets`

CreativeLocalizationWithAssets.AppPreviewDeviceWithAssets

The map of available app preview details for a device.

`deviceClasses`

`string`

The device classes assigned to a custom product page.

See DeviceClass for value descriptions.

Possible Values: `IPAD, IPHONE`

`language`

`string`

The language associated with the ISO alpha-2 country code, such as `US`.

`languageCode`

`string`

The ISO 639-1 language code appended to the ISO alpha-2 country code, such as `en-US`.

`promotionalText`

`string`

Text that appears at the top of the main description of a product page.

`shortDescription`

`string`

Concise, informative text to describe an app on a product page.

`subTitle`

`string`

A summary of an app that appears below the name of an app on a product page.

## Topics

### Objects

object CreativeLocalizationWithAssets.AppPreviewDeviceWithAssets

A map of app preview device assets.

## See Also

### Creative Request and Response Objects

object AppPreviewDevicesMappingResponse

The app preview device mapping response to display name and size mapping requests.

object Creative

The creative object.

object CreativeLocalization

The localized creative metadata.

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

