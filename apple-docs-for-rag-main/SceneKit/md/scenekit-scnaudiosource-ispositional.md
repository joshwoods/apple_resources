

- SceneKit
- SCNAudioSource
-  isPositional 

Instance Property

# isPositional

A Boolean value that determines whether audio from this source uses 3D positional mixing.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isPositional: Bool { get set }
```

## Discussion

If this value is true (the default), SceneKit mixes audio from the source based on its position relative to the scene’s audioListener node—that is, the audio source’s volume, reverb, and other parameters automatically change depending on the distance to the listener and other objects in the scene. (To position an audio source in a scene, create an SCNAudioPlayer player from the source and attach that player to an SCNNode object.)

If you set this property to false, the source’s audio plays with the same volume (and other mixing parameters) regardless of the listener’s position.

