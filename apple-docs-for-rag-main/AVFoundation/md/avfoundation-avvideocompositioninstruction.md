

- AVFoundation
-  AVVideoCompositionInstruction 

Class

# AVVideoCompositionInstruction

An operation that a compositor performs.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVVideoCompositionInstruction
```

## Overview

An AVVideoComposition object maintains an array of instructions to perform its composition.

## Topics

### Inspecting the Instruction

var backgroundColor: CGColor?

The background color of the composition.

var layerInstructions: [AVVideoCompositionLayerInstruction]

Instructions that specify how to layer and compose video frames from source tracks.

var timeRange: CMTimeRange

The time range to which the instruction applies.

var enablePostProcessing: Bool

A Boolean value that indicates whether the instruction requires post processing.

### Identifying Source Tracks

var requiredSourceTrackIDs: [NSValue]

The identifiers of source video tracks that the compositor requires to compose frames for the instruction.

var requiredSourceSampleDataTrackIDs: [NSNumber]

The identifiers of source sample data tracks that the compositor requires to compose frames for the instruction.

var passthroughTrackID: CMPersistentTrackID

The track identifier from an instruction source frame.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableVideoCompositionInstruction

### Conforms To

- AVVideoCompositionInstructionProtocol
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

class AVMutableVideoCompositionInstruction

A mutable video composition instruction subclass.

class AVVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a composition.

class AVMutableVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a mutable composition.

