

- AVFAudio
- AVAudioEnvironmentNode
-  listenerVectorOrientation 

Instance Property

# listenerVectorOrientation

The listener’s vector orientation in the environment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var listenerVectorOrientation: AVAudio3DVectorOrientation { get set }
```

## Discussion

The default orientation is with the listener looking directly along the negative z-axis (forward).

The node expresses a forward vector orientation as `(0, 0, -1)`, and an up vector as `(0, 1, 0)`.

Changing this property results in a corresponding change in the listenerAngularOrientation property.

## See Also

### Getting and Setting Positional Properties

var listenerPosition: AVAudio3DPoint

The listener’s position in the 3D environment.

var listenerAngularOrientation: AVAudio3DAngularOrientation

The listener’s angular orientation in the environment.

