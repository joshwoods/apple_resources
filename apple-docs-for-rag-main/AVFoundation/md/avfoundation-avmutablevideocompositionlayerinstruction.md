

- AVFoundation
-  AVMutableVideoCompositionLayerInstruction 

Class

# AVMutableVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a mutable composition.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVMutableVideoCompositionLayerInstruction
```

## Topics

### Creating an Instruction

convenience init(assetTrack: AVAssetTrack)

Creates a new mutable video composition layer instruction for the given track.

### Configuring a Track ID

var trackID: CMPersistentTrackID

The track identifier of the source track to which the compositor applies the instruction.

### Managing Properties

func setOpacity(Float, at: CMTime)

Sets the opacity value at a specific time within the time range of the instruction.

func setOpacityRamp(fromStartOpacity: Float, toEndOpacity: Float, timeRange: CMTimeRange)

Sets an opacity ramp to apply during a specified time range.

func setTransform(CGAffineTransform, at: CMTime)

Sets the transform value at a time within the time range of the instruction.

func setTransformRamp(fromStart: CGAffineTransform, toEnd: CGAffineTransform, timeRange: CMTimeRange)

Sets a transform ramp to apply during a given time range.

### Setting Crop Rectangle Values

func setCropRectangle(CGRect, at: CMTime)

Sets the crop rectangle value at a time within the time range of the instruction.

func setCropRectangleRamp(fromStartCropRectangle: CGRect, toEndCropRectangle: CGRect, timeRange: CMTimeRange)

Sets a crop rectangle ramp to apply during the specified time range.

## Relationships

### Inherits From

- AVVideoCompositionLayerInstruction

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

class AVVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a composition.

