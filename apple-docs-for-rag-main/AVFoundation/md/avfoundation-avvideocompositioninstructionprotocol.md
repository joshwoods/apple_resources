

- AVFoundation
-  AVVideoCompositionInstructionProtocol 

Protocol

# AVVideoCompositionInstructionProtocol

A protocol that defines the interface for a video composition instruction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
protocol AVVideoCompositionInstructionProtocol : NSObjectProtocol
```

## Overview

A video composition maintains an array of instructions that describe how to compose its content.

## Topics

### Getting Track ID Settings

var passthroughTrackID: CMPersistentTrackID

An identifier of a source track to pass through without compositing.

**Required**

var requiredSourceTrackIDs: [NSValue]?

The identifiers of the video tracks the instruction requires to compose frames.

**Required**

var requiredSourceSampleDataTrackIDs: [NSNumber]

The identifiers of the sample data tracks the instruction requires to compose frames.

### Getting Tweening Settings

var containsTweening: Bool

A Boolean value that indicates whether the composition contains tweening.

**Required**

### Getting Post-Processing Status

var enablePostProcessing: Bool

A Boolean value that indicates whether the composition enables post-processing.

**Required**

### Getting Timing Settings

var timeRange: CMTimeRange

The time range during which the instruction is effective.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- AVMutableVideoCompositionInstruction
- AVVideoCompositionInstruction

## See Also

### Specifying composition instructions

var instructions: [any AVVideoCompositionInstructionProtocol]

The video composition instructions.

