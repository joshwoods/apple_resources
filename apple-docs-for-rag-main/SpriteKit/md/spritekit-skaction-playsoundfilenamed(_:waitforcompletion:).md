

- SpriteKit
- SKAction
-  playSoundFileNamed(\_:waitForCompletion:) 

Type Method

# playSoundFileNamed(\_:waitForCompletion:)

Creates an action that plays a sound.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func playSoundFileNamed(
    _ soundFile: String,
    waitForCompletion wait: Bool
) -> SKAction
```

## Parameters 

`soundFile`  

The name of a sound file in the app’s bundle.

`wait`  

If true, the duration of this action is the same as the length of the audio playback. If false, the action is considered to have completed immediately.

## Return Value

A new action object.

## Discussion

Use SKAction `playSoundFileNamed:waitForCompletion:` only for short incidentals. Use AVAudioPlayer for long running background music. This action is not reversible; the reversed action is identical to the original action.

## See Also

### Controlling the Audio of a Node

class func play() -> SKAction

Creates an action that tells an audio node to start playback.

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

