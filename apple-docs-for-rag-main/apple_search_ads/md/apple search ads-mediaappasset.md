

- Apple Search Ads
-  MediaAppAsset 

Object

# MediaAppAsset

The asset details of app preview or app screenshots.

Search Ads 4.0+

``` source
object MediaAppAsset
```

## Properties

`assetGenId`

`string`

The unique identifier for the app preview or screenshot.

Your `adamId` is the first numerical grouping in `assetGenId`. For example, in `1408851466;en-US;5;0;f8c9add6280c781e6f701c506be5a921`, `1408851466` is your `adamId`.

`assetType`

`string`

The type of creative asset.

App previews are still images of video assets that you upload to App Store Connect. Note, the playable URL isn’t in the API response.

A screenshot is a standard image of the app that you upload to App Store Connect.

Possible Values: `APP_PREVIEW, SCREENSHOT`

`assetURL`

`string`

The resolved URL for the screenshot or a screenshot of the video asset.

`orientation`

`string`

The orientation of the asset that you upload to App Store Connect.

Possible Values: `LANDSCAPE, PORTRAIT, UNKNOWN`

`sortPosition`

`int64`

The position of the asset that you upload to App Store Connect.

`sourceHeight`

`int32`

The height of the asset that you upload to App Store Connect.

`sourceWidth`

`int32`

The width of the asset that you upload to App Store Connect.

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

object MediaAppAssetsDetail

The app asset details of a device.

