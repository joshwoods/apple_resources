

- ImageCaptureCore
- ICCameraFile
-  pairedRawImage 

Instance Property

# pairedRawImage

A sidecar file containing the logical `RAW` compliment of a `JPG` or other two-format image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var pairedRawImage: ICCameraFile? { get }
```

## Discussion

This value contains a single-item subset of the sidecarFiles array.

## See Also

### Identifying Related Files

var sidecarFiles: [ICCameraItem]?

An array of two camera files associated with this file.

