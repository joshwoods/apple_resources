

- PHASE
- PHASESource
-  gain 

Instance Property

# gain

The amount of sound the source emanates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var gain: Double { get set }
```

## Discussion

The framework clamps the value to the range between `0` and `1`, where `0` silences the audio and `1` doesn’t modify the audio’s original volume.

