

- PHASE
-  PHASEPushStreamBufferOptions 

Structure

# PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct PHASEPushStreamBufferOptions
```

## Overview

When your app provides audio buffers that PHASE plays through a PHASEPushStreamNode, use this structure to inform PHASE of a particular buffer’s priority.

Associate an option to a particular buffer by passing it in to the scheduleBuffer(buffer:time:options:) function of a PHASEPushStreamNode.

## Topics

### Creating an Option

init(rawValue: UInt)

Creates a push stream buffer option with the given raw value.

### Options

static var `default`: PHASEPushStreamBufferOptions

Indicates a buffer processes after existing buffers in the queue.

static var interrupts: PHASEPushStreamBufferOptions

Indicates a buffer begins processing immediately.

static var interruptsAtLoop: PHASEPushStreamBufferOptions

Indicates a buffer begins processing when an existing buffer loops.

static var loops: PHASEPushStreamBufferOptions

Indicates a buffer restarts after it finishes processing.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Audio-Providing Nodes

class PHASESamplerNodeDefinition

A node that plays complete audio data.

enum PHASEPlaybackMode

Loop options for audio playback.

class PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

class PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

enum PHASECalibrationMode

Calibration options for sound pressure level.

class PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

