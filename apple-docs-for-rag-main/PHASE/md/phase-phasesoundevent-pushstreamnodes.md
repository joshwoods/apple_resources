

- PHASE
- PHASESoundEvent
-  pushStreamNodes 

Instance Property

# pushStreamNodes

A collection of audio streams for playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var pushStreamNodes: [String : PHASEPushStreamNode] { get }
```

## Discussion

This dictionary populates a push-stream node for sound events that PHASE generates for PHASEPushStreamNodeDefinition in your event node tree. The dictionary key is the stream-node definition’s identifier.

