

- AVFAudio
- AVAudioConnectionPoint
-  bus 

Instance Property

# bus

The bus on the node in the connection point.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bus: AVAudioNodeBus { get }
```

## See Also

### Getting Connection Point Properties

func inputConnectionPoint(for: AVAudioNode, inputBus: AVAudioNodeBus) -> AVAudioConnectionPoint?

Returns connection information about a node’s input bus.

func outputConnectionPoints(for: AVAudioNode, outputBus: AVAudioNodeBus) -> [AVAudioConnectionPoint]

Returns connection information about a node’s output bus.

var node: AVAudioNode?

The node in the connection point.

