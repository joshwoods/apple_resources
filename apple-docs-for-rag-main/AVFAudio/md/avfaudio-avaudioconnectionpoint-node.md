

- AVFAudio
- AVAudioConnectionPoint
-  node 

Instance Property

# node

The node in the connection point.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var node: AVAudioNode? { get }
```

## See Also

### Getting Connection Point Properties

func inputConnectionPoint(for: AVAudioNode, inputBus: AVAudioNodeBus) -> AVAudioConnectionPoint?

Returns connection information about a node’s input bus.

func outputConnectionPoints(for: AVAudioNode, outputBus: AVAudioNodeBus) -> [AVAudioConnectionPoint]

Returns connection information about a node’s output bus.

var bus: AVAudioNodeBus

The bus on the node in the connection point.

