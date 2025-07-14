

- PHASE
- PHASESpatializationMode
-  PHASESpatializationMode.automatic 

Case

# PHASESpatializationMode.automatic

A mode that indicates that the framework chooses the spatialization mode.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
case automatic
```

## Discussion

This setting instructs the framework to automatically set a mode that determines how PHASE positions and orients sound in 3D space. The framework chooses a mode based on the output device:

`PHASESpatializationMode.binaural`  
Headphones (Bluetooth or line output) and the internal speakers of supported Mac or iOS devices.

`PHASESpatializationMode.channelBased`  
External speakers with 2 or more channels.

## See Also

### Modes

case alwaysUseBinaural

A mode that introduces special processing to replicate a realistic spatial listening experience.

case alwaysUseChannelBased

A mode that adds a 3D position and orientation to sound by panning across the available output channels.

