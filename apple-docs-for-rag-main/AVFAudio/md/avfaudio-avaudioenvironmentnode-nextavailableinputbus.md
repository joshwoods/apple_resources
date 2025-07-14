

- AVFAudio
- AVAudioEnvironmentNode
-  nextAvailableInputBus 

Instance Property

# nextAvailableInputBus

An unused input bus.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var nextAvailableInputBus: AVAudioNodeBus { get }
```

## Discussion

This method finds and returns the first input bus that doesn’t have a connection with a node.

