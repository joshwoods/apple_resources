

- ImageCaptureCore
- ICCameraFile
-  orientation 

Instance Property

# orientation

The orientation to use when downloading the image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var orientation: ICEXIFOrientationType { get set }
```

## Discussion

This property is initially set to ICEXIFOrientationType.orientation1 If the format of the file supports the `EXIF` orientation tag, then this property updates to match the value of that tag on receipt of the thumbnail or metadata for this file.

## See Also

### Inspecting a File’s EXIF Data

enum ICEXIFOrientationType

The file’s orientation type.

var exifCreationDate: Date?

The `EXIF` creation date of the file.

var exifModificationDate: Date?

The `EXIF` modification date of the file.

