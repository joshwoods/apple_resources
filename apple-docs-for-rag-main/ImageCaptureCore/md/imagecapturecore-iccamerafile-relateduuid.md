

- ImageCaptureCore
- ICCameraFile
-  relatedUUID 

Instance Property

# relatedUUID

A related UUID correlating several images from an Apple device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var relatedUUID: String? { get }
```

## Discussion

This value is the same for both the image and video of a LivePhoto.

## See Also

### Inspecting a File's Identity

var groupUUID: String?

The group `UUID` of the file.

var originatingAssetID: String?

The originating asset ID of an `HEIF` or `HVEC` file.

