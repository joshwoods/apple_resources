

- Apple Search Ads
-  AppAsset 

Object

# AppAsset

The app assets associated with an adam ID.

Search Ads 4.8+

``` source
object AppAsset
```

## Properties

`adamId`

`string`

Your unique App Store app identifier. Use Get a Campaign or Get all Campaigns to obtain your `adamId`.

You can use the `EQUALS` and `IN` Selector Condition operators with Find App Assets.

This field is sortable.

`appPreviewDevice`

`string`

Indicates the device model and corresponding display size. See AppPreviewDevicesMappingResponse.Data.

This field is sortable.

`assetGenId`

`string`

The unique identifier for an app preview or screenshot.

Your `adamId` is the first numerical grouping in `assetGenId`. For example, in `1408851466;en-US;5;0;f8c9add6280c781e6f701c506be5a921`, `1408851466` is your `adamId`.

You can use the `EQUALS` and `IN` Selector Condition operators with Find App Assets.

This field is sortable.

`assetType`

`string`

The type of creative asset.

`APP_PREVIEW` is a video still image of video assets that you upload to App Store Connect. Note, the playable URL isn’t in the API response.

`SCREENSHOT` is a standard image of the app that you upload to App Store Connect.

Possible Values: `APP_PREVIEW, SCREENSHOT`

`assetURL`

`string`

The resolved URL for the screenshot that you upload to App Store Connect. For a video asset, the image is the first frame.

`assetVideoUrl`

`string`

The fully resolved URL for the asset video. The field is non-null for preview assets; otherwise, it’s null.

`deleted`

`boolean`

Indicates whether the asset was deleted from App Store Connect.

This field is sortable.

`orientation`

`string`

The orientation of the asset that you upload to App Store Connect.

Possible Values: `LANDSCAPE, PORTRAIT, UNKNOWN`

`sourceHeight`

`int32`

The height of the asset that you upload to App Store Connect.

This field is sortable.

`sourceWidth`

`int32`

The width of the asset that you upload to App Store Connect.

This field is sortable.

## See Also

### Ad Rejection Reason Objects

object AppAssetListResponse

The response to a request that returns a list of app assets.

object ProductPageReason

The ad creative rejection reason based on a product page.

object ProductPageReasonListResponse

The response to a request that returns a list of product page rejection reasons.

object ProductPageReasonResponse

A container for product page reasons.

