

- Core Media
-  kCMMetadataIdentifier_QuickTimeMetadataPreferredAffineTransform 

Global Variable

# kCMMetadataIdentifier_QuickTimeMetadataPreferredAffineTransform

An affine transform to be applied to a video track.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMMetadataIdentifier_QuickTimeMetadataPreferredAffineTransform: CFString
```

## Discussion

This affine transform can be used in place of a track matrix for displaying a video track to better reflect the current orientation of a video camera with respect to a scene. For example, if the camera is rotated after a recording has started, the presence of this metadata will allow a player to adjust its rendering at the time the rotation occurred.

## See Also

### Constants

let kCMMetadataIdentifier_QuickTimeMetadataLocation_ISO6709: CFString

Location information in ISO-6709 format.

let kCMMetadataIdentifier_QuickTimeMetadataDirection_Facing: CFString

Direction the observer is facing.

let kCMMetadataIdentifier_QuickTimeMetadataVideoOrientation: CFString

Video orientation as defined by TIFF/EXIF.

let kCMMetadataIdentifier_QuickTimeMetadataLivePhotoStillImageTransformReferenceDimensions: CFString

The dimensions of the live photo still image.

let kCMMetadataIdentifier_QuickTimeMetadataLivePhotoStillImageTransform: CFString

A perspective transform you use to adjust a Live Photo still image to match the Live Photo movie.

