

- Apple Search Ads
-  MediaAppAssetsDetail 

Object

# MediaAppAssetsDetail

The app asset details of a device.

Search Ads 4.0+

``` source
object MediaAppAssetsDetail
```

## Properties

`appPreviewDeviceFallBackDevices`

`[string]`

Devices that don’t have uploaded assets use fallback device mapping.

`appPreviews`

`[`MediaAppVideoAsset`]`

Still images of video assets to use for app previews.

`screenshots`

`[`MediaAppAsset`]`

Standard images of your app to use for app previews.

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

object DefaultProductPageCreative

The default product page object.

object MediaAppAsset

The asset details of app preview or app screenshots.

