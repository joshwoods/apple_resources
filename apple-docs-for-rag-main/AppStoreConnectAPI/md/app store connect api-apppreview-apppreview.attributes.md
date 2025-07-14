

- App Store Connect API
- AppPreview
-  AppPreview.Attributes 

Object

# AppPreview.Attributes

Attributes that describe an App Previews resource.

App Store Connect API 1.2+

``` source
object AppPreview.Attributes
```

## Properties

`assetDeliveryState`

AppMediaAssetState

This attribute is deprecated. Use AppMediaVideoState instead.

`fileName`

`string`

`fileSize`

`integer`

`mimeType`

`string`

`previewFrameImage`

PreviewFrameImage

`previewFrameTimeCode`

`string`

`previewImage`

ImageAsset

This attribute is deprecated. Use PreviewFrameImage instead.

`sourceFileChecksum`

`string`

`uploadOperations`

`[`UploadOperation`]`

`videoDeliveryState`

AppMediaVideoState

`videoUrl`

`string`

## Mentioned in 

App Store Connect API 3.7 release notes

## See Also

### Objects

object AppPreview.Relationships

The relationships you included in the request and those on which you can operate.

