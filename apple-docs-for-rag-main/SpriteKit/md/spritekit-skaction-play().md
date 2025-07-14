

- SpriteKit
- SKAction
-  play() 

Type Method

# play()

Creates an action that tells an audio node to start playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func play() -> SKAction
```

## Return Value

A new action object.

## Discussion

This action may only be executed on an SKAudioNode object.

This action is not reversible.

## See Also

### Controlling the Audio of a Node

class func playSoundFileNamed(String, waitForCompletion: Bool) -> SKAction

Creates an action that plays a sound.

class func pause() -> SKAction

Creates an action that tells an audio node to pause playback.

class func stop() -> SKAction

Creates an action that tells an audio node to stop playback.

class func changePlaybackRate(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s playback rate to a new value.

class func changePlaybackRate(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s playback rate by a relative amount.

class func changeVolume(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s volume to a new value.

class func changeVolume(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s volume by a relative value.

class func changeObstruction(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s obstruction to a new value.

class func changeObstruction(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s obstruction by a relative value.

class func changeOcclusion(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s occlusion to a new value.

class func changeOcclusion(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s occlusion by a relative value.

class func changeReverb(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s reverb to a new value.

class func changeReverb(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s reverb by a relative value.

class func stereoPan(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s stereo panning to a new value.

class func stereoPan(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s stereo panning by a relative value.

