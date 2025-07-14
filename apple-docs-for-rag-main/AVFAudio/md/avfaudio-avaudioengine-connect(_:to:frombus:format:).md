

- AVFAudio
- AVAudioEngine
-  connect(\_:to:fromBus:format:) 

Instance Method

# connect(\_:to:fromBus:format:)

Establishes a connection between a source node and multiple destination nodes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func connect(
    _ sourceNode: AVAudioNode,
    to destNodes: [AVAudioConnectionPoint],
    fromBus sourceBus: AVAudioNodeBus,
    format: AVAudioFormat?
)
```

## Parameters 

`sourceNode`  

The source node.

`destNodes`  

An array of AVAudioConnectionPoint objects that specify destination nodes and busses.

`sourceBus`  

The output bus on the source node.

`format`  

If not `NULL`, the framework uses this value for the format of the source audio node’s output bus. In all cases, the framework matches the format of the destination audio node’s input bus to the source audio node’s output bus.

## Discussion

Connections that use this method are either one-to-one or one-to-many.

## See Also

### Using Connection Points

class AVAudioConnectionPoint

A representation of either a source or destination connection point in the audio engine.

