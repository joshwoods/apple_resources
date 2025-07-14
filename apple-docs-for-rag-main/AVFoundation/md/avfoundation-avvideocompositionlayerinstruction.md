

- AVFoundation
-  AVVideoCompositionLayerInstruction 

Class

# AVVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a composition.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVVideoCompositionLayerInstruction
```

## Topics

### Getting the Track ID

var trackID: CMPersistentTrackID

The track identifier of the source track to which the compositor will apply the instruction.

### Getting Opacity, Transform, and Cropping Ramps

func getOpacityRamp(for: CMTime, startOpacity: UnsafeMutablePointer&lt;Float>?, endOpacity: UnsafeMutablePointer&lt;Float>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the opacity ramp that includes a specified time.

func getTransformRamp(for: CMTime, start: UnsafeMutablePointer&lt;CGAffineTransform>?, end: UnsafeMutablePointer&lt;CGAffineTransform>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the transform ramp that includes a specified time.

func getCropRectangleRamp(for: CMTime, startCropRectangle: UnsafeMutablePointer&lt;CGRect>?, endCropRectangle: UnsafeMutablePointer&lt;CGRect>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Obtains the crop rectangle ramp that includes the specified time.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableVideoCompositionLayerInstruction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Built-in video compositing

Editing and Playing HDR Video

Support high-dynamic-range (HDR) video content in your app by using the HDR editing and playback capabilities of AVFoundation.

Debugging AVFoundation audio mixes, compositions, and video compositions

Resolve common problems when creating compositions, video compositions, and audio mixes.

class AVVideoComposition

An object that describes how to compose video frames at particular points in time.

class AVMutableVideoComposition

A mutable video composition subclass.

class AVVideoCompositionInstruction

An operation that a compositor performs.

class AVMutableVideoCompositionInstruction

A mutable video composition instruction subclass.

class AVMutableVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a mutable composition.

