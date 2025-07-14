

- AVFAudio
- AVAudioEngine
-  outputConnectionPoints(for:outputBus:) 

Instance Method

# outputConnectionPoints(for:outputBus:)

Returns connection information about a node’s output bus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func outputConnectionPoints(
    for node: AVAudioNode,
    outputBus bus: AVAudioNodeBus
) -> [AVAudioConnectionPoint]
```

## Parameters 

`node`  

The node with the output connections you’re querying.

`bus`  

The node’s output bus for connections you’re querying.

## Return Value

An array of `AVAudioConnectionPoint` objects with connection information on the node’s output bus.

## Discussion

Connections are always one-to-one or one-to-many. This method returns an empty array if there are no connections on the node’s specified output bus.

## See Also

### Getting Connection Point Properties

func inputConnectionPoint(for: AVAudioNode, inputBus: AVAudioNodeBus) -> AVAudioConnectionPoint?

Returns connection information about a node’s input bus.

var bus: AVAudioNodeBus

The bus on the node in the connection point.

var node: AVAudioNode?

The node in the connection point.

