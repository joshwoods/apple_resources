

- AVFoundation
- AVPartialAsyncProperty
-  naturalSize 

Type Property

# naturalSize

The natural dimensions of the media data that the track references.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var naturalSize: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

For visual tracks, like video or subtitle tracks, this property value is the natural size of the media. For nonvisual tracks, like audio or chapter tracks, the value is zero.

## See Also

### Loading Visual Characteristics

static var preferredTransform: AVAsyncProperty&lt;Root, CGAffineTransform>

The track’s transform preference to apply to its visual content during presentation or processing.

