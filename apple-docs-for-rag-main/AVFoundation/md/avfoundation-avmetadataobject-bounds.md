

- AVFoundation
- AVMetadataObject
-  bounds 

Instance Property

# bounds

The bounding rectangle associated with the metadata.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
var bounds: CGRect { get }
```

## Discussion

The bounding rectangle is specified relative to the picture or video of the corresponding media. The rectangle’s origin is always specified in the top-left corner, and the x and y axis extend down and to the right.

If the metadata has no bounding rectangle, the value of this property should be CGRectZero.

For video content, the bounding rectangle may be expressed using scalar values in the range 0.0 to 1.0. Scalar values remain meaningful even when the original video has been scaled down.

## See Also

### Getting the Media-Related Attributes

var time: CMTime

The media time value associated with the metadata object.

var duration: CMTime

The duration of the media associated with this metadata object.

