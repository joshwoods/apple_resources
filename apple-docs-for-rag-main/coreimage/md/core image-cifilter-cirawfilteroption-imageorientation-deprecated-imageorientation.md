

- Core Image
- CIFilter
- CIRAWFilterOption
-  imageOrientation Deprecated

Type Property

# imageOrientation

A key for the image orientation. The associated value is an integer value packaged as an NSNumber object. Valid values are in range `1...8` and follow the EXIF specification. The value is disregarded when the `kCIIgnoreImageOrientationKey` flag is set. You can change the orientation of the image by overriding this value. By changing this value you can rotate an image in 90-degree increments.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let imageOrientation: CIRAWFilterOption
```

