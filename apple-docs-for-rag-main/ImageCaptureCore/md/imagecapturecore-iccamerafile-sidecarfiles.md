

- ImageCaptureCore
- ICCameraFile
-  sidecarFiles 

Instance Property

# sidecarFiles

An array of two camera files associated with this file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var sidecarFiles: [ICCameraItem]? { get }
```

## Discussion

An example of a sidecar file is a file with the same base 3 name as this file and an `XMP` extension.

## See Also

### Identifying Related Files

var pairedRawImage: ICCameraFile?

A sidecar file containing the logical `RAW` compliment of a `JPG` or other two-format image.

