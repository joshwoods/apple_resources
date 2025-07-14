

- SceneKit
- SCNAction
-  playAudio(\_:waitForCompletion:) 

Type Method

# playAudio(\_:waitForCompletion:)

Creates an action that plays an audio source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func playAudio(
    _ source: SCNAudioSource,
    waitForCompletion wait: Bool
) -> SCNAction
```

## Parameters 

`source`  

The audio source to play.

`wait`  

If true, the duration of this action is the same as the length of the audio playback. If false, the action is considered to have completed immediately.

## Return Value

A new action object.

## Discussion

When the action executes, SceneKit plays the audio source on the target node—any positional audio effects are based on the node’s position. For more information about positional audio in SceneKit, see SCNAudioPlayer.

This action is not reversible; the reverse of this action is the same action.

