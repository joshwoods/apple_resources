

- PHASE
- PHASEListener
-  gain 

Instance Property

# gain

Modifies the volume of all audio playback for the listener’s mixers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var gain: Double { get set }
```

## Discussion

For mixers that require a listener, this property modifies the volume of all audio the framework plays back through the listener by way of the listener’s associated mixers. The framework clamps the value to the range between `0` and `1`, where `0` silences the audio and `1` doesn’t modify the audio’s original volume.

