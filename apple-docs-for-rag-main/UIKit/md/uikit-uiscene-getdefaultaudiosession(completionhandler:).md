

- UIKit
- UIScene
-  getDefaultAudioSession(completionHandler:) 

Instance Method

# getDefaultAudioSession(completionHandler:)

Retrieves the audio session that contains all sounds that implicitly belong to this scene.

visionOS 1.0+

``` source
nonisolated
func getDefaultAudioSession(completionHandler handler: @escaping (AVAudioSession?) -> Void)
```

``` source
nonisolated
var defaultAudioSession: AVAudioSession? { get async }
```

## Discussion

In visionOS, the default AVAudioSession for a UIScene contains all of the RealityKit sounds from any RealityView in the scene’s view hierarchy.

The default audio session’s initial configuration is mixable, with isNowPlayingCandidate set to false. This configuration ensures that the scene’s default audio session doesn’t interfere with existing behavior of the app’s primary audio session, sharedInstance(). However, you can modify the default audio session’s properties as needed.

You can safely call this method on a non-main thread. It’s recommended to get a scene’s default audio session from a non-main thread to avoid calling resource-intensive AVAudioSession interfaces from the main thread, which can have a negative impact on the responsiveness of the user experience.

