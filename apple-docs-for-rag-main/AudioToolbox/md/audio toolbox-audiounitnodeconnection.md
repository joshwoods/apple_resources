

- Audio Toolbox
-  AudioUnitNodeConnection 

Structure

# AudioUnitNodeConnection

A connection between two node objects in an audio processing graph.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitNodeConnection
```

## Topics

### Initializers

init()

init(sourceNode: AUNode, sourceOutputNumber: UInt32, destNode: AUNode, destInputNumber: UInt32)

### Instance Properties

var destInputNumber: UInt32

var destNode: AUNode

var sourceNode: AUNode

var sourceOutputNumber: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

typealias AUGraph

An opaque type representing an audio processing graph.

typealias AUNode

A member of an audio processing graph, associated with an audio unit.

struct AUNodeInteraction

Describes the interaction between two node objects.

struct AUNodeRenderCallback

A callback used to provide input to an audio unit.

