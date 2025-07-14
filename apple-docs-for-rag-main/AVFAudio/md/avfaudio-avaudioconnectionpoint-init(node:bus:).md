

- AVFAudio
- AVAudioConnectionPoint
-  init(node:bus:) 

Initializer

# init(node:bus:)

Creates a connection point object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    node: AVAudioNode,
    bus: AVAudioNodeBus
)
```

## Parameters 

`node`  

The source or destination node.

`bus`  

The output or input bus on the node.

## Discussion

If the node is `nil`, this method fails and returns `nil`.

