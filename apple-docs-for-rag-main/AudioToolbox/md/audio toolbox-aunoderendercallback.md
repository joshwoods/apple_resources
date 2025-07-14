

- Audio Toolbox
-  AUNodeRenderCallback 

Structure

# AUNodeRenderCallback

A callback used to provide input to an audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AUNodeRenderCallback
```

## Overview

Used to contain information when a callback is used to provide input to the specific node’s specified input.

## Topics

### Initializers

init()

init(destNode: AUNode, destInputNumber: AudioUnitElement, cback: AURenderCallbackStruct)

### Instance Properties

var cback: AURenderCallbackStruct

var destInputNumber: AudioUnitElement

var destNode: AUNode

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct AudioUnitNodeConnection

A connection between two node objects in an audio processing graph.

typealias AUGraph

An opaque type representing an audio processing graph.

typealias AUNode

A member of an audio processing graph, associated with an audio unit.

struct AUNodeInteraction

Describes the interaction between two node objects.

