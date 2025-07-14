

- Apple Search Ads
-  CreativeLocalization 

Object

# CreativeLocalization

The localized creative metadata.

Search Ads 4.0+

``` source
object CreativeLocalization
```

## Properties

`appName`

`string`

The app name on App Store Connect.

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

## See Also

### Creative Request and Response Objects

object AppPreviewDevicesMappingResponse

The app preview device mapping response to display name and size mapping requests.

object Creative

The creative object.

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

