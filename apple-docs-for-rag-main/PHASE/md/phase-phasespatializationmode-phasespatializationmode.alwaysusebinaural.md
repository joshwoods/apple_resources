

- PHASE
- PHASESpatializationMode
-  PHASESpatializationMode.alwaysUseBinaural 

Case

# PHASESpatializationMode.alwaysUseBinaural

A mode that introduces special processing to replicate a realistic spatial listening experience.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case alwaysUseBinaural
```

## Discussion

Enable this mode to override a system or user preference and implement binaural audio output. When binaural mode plays through internal speakers on supported Apple devices, the framework applies additional effects to the output to achieve a sound experience comparable to one with headphones.

## See Also

### Modes

case automatic

A mode that indicates that the framework chooses the spatialization mode.

case alwaysUseChannelBased

A mode that adds a 3D position and orientation to sound by panning across the available output channels.

