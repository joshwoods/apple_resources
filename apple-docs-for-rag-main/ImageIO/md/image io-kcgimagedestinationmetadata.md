

- Image I/O
-  kCGImageDestinationMetadata 

Global Variable

# kCGImageDestinationMetadata

The metadata tags to include with the image.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImageDestinationMetadata: CFString
```

## Discussion

The value of this key is a CGImageMetadata type. When you specify this key, the image destination ovewrites all EXIF, IPTC, and XMP metadata. If you want to merge the new tags with the existing metadata, include the kCGImageDestinationMergeMetadata key in addition to this key.

## See Also

### Configuring the Image Behaviors

let kCGImageDestinationLossyCompressionQuality: CFString

The desired compression quality to use when writing the image data.

let kCGImageDestinationBackgroundColor: CFString

The background color to use when the image has an alpha component, but the destination format doesn’t support alpha.

let kCGImageDestinationDateTime: CFString

The date and time information to associate with the image.

let kCGImageDestinationEmbedThumbnail: CFString

A Boolean value that indicates whether to embed a thumbnail for JPEG and HEIF images.

let kCGImageDestinationImageMaxPixelSize: CFString

The maximum width and height of the image, in pixels.

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

