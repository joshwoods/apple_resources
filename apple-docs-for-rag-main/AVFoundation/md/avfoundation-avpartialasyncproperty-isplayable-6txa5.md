

- AVFoundation
- AVPartialAsyncProperty
-  isPlayable 

Type Property

# isPlayable

A Boolean value that indicates whether the track is playable in the current environment.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var isPlayable: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Track Information

static var formatDescriptions: AVAsyncProperty&lt;Root, [CMFormatDescription]>

The format descriptions of the media samples that a track references.

static var isDecodable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is decodable in the current environment.

static var isEnabled: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is in an enabled state.

static var isSelfContained: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track references sample data only within its container file.

static var totalSampleDataLength: AVAsyncProperty&lt;Root, Int64>

The total number of bytes of sample data the track requires.

static var mediaCharacteristics: AVAsyncProperty&lt;Root, [AVMediaCharacteristic]>

The media characteristics for the track.

