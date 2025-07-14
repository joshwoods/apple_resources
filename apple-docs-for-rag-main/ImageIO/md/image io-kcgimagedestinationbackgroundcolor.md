

- Image I/O
-  kCGImageDestinationBackgroundColor 

Global Variable

# kCGImageDestinationBackgroundColor

The background color to use when the image has an alpha component, but the destination format doesn’t support alpha.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageDestinationBackgroundColor: CFString
```

## Discussion

If present, the value associated with this key must be a CGColor data type without an alpha component of its own. If not present, and if a background color is needed, a white color is used.

## See Also

### Configuring the Image Behaviors

let kCGImageDestinationLossyCompressionQuality: CFString

The desired compression quality to use when writing the image data.

let kCGImageDestinationDateTime: CFString

The date and time information to associate with the image.

let kCGImageDestinationEmbedThumbnail: CFString

A Boolean value that indicates whether to embed a thumbnail for JPEG and HEIF images.

let kCGImageDestinationImageMaxPixelSize: CFString

The maximum width and height of the image, in pixels.

let kCGImageDestinationMetadata: CFString

The metadata tags to include with the image.

let kCGImageDestinationMergeMetadata: CFString

A Boolean value that indicates whether to merge new metadata with the image’s existing metadata.

let kCGImageDestinationOptimizeColorForSharing: CFString

A Boolean value that indicates whether to create the image using a colorspace.

let kCGImageDestinationOrientation: CFString

The orientation of the image, specified as an EXIF value in the range 1 to 8.

let kCGImageDestinationPreserveGainMap: CFString

A Boolean value that indicates whether to include a HEIF-embedded gain map in the image data.

let kCGImageMetadataShouldExcludeGPS: CFString

A Boolean value that indicates whether to exclude GPS metadata from EXIF data or the corresponding XMP tags.

let kCGImageMetadataShouldExcludeXMP: CFString

A Boolean value that indicates whether to exclude XMP data from the destination.

