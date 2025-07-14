

- PHASE
- PHASESpatializationMode
-  PHASESpatializationMode.alwaysUseChannelBased 

Case

# PHASESpatializationMode.alwaysUseChannelBased

A mode that adds a 3D position and orientation to sound by panning across the available output channels.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case alwaysUseChannelBased
```

## Discussion

The framework selects a channel layout for the output audio that’s compatible with the device’s channel configuration in Settings.

This mode applies the same effect regardless of the current output device.

## See Also

### Modes

case automatic

A mode that indicates that the framework chooses the spatialization mode.

case alwaysUseBinaural

A mode that introduces special processing to replicate a realistic spatial listening experience.

