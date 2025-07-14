

- AVFAudio
- AVAudioEngine
-  inputConnectionPoint(for:inputBus:) 

Instance Method

# inputConnectionPoint(for:inputBus:)

Returns connection information about a node’s input bus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func inputConnectionPoint(
    for node: AVAudioNode,
    inputBus bus: AVAudioNodeBus
) -> AVAudioConnectionPoint?
```

## Parameters 

`node`  

The node with the input connection you’re querying.

`bus`  

The node’s input bus for the connection you’re querying.

## Return Value

An `AVAudioConnectionPoint` object with connection information on the node’s input bus.

## Discussion

Connections are always one-to-one or one-to-many. This method returns `nil` if there’s no connection on the node’s specified input bus.

## See Also

### Getting Connection Point Properties

func outputConnectionPoints(for: AVAudioNode, outputBus: AVAudioNodeBus) -> [AVAudioConnectionPoint]

Returns connection information about a node’s output bus.

var bus: AVAudioNodeBus

The bus on the node in the connection point.

var node: AVAudioNode?

The node in the connection point.

