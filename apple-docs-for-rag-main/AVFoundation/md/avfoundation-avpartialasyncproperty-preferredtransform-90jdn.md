

- AVFoundation
- AVPartialAsyncProperty
-  preferredTransform 

Type Property

# preferredTransform

The track’s transform preference to apply to its visual content during presentation or processing.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var preferredTransform: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Visual Characteristics

static var naturalSize: AVAsyncProperty&lt;Root, CGSize>

The natural dimensions of the media data that the track references.

