

- SceneKit
- SCNAudioPlayer
-  audioSource 

Instance Property

# audioSource

The source of audio played by this player.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var audioSource: SCNAudioSource? { get }
```

## Discussion

An SCNAudioSource object represents a distinct source of audio—for example, a sound file—that can be reused and shared by many player objects. Use a player’s audio source to configure the default values for playback parameters such as volume and reverb. To vary those parameters in real time during playback, use the audioNode property to work with the underlying AVAudioNode object.

If the player was created with the audioPlayerWithAVAudioNode: method, this property’s value is `nil`.

## See Also

### Working with Audio Sources

var audioNode: AVAudioNode?

The audio node SceneKit uses for mixing audio from this player.

