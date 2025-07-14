

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClassID
-  LFEVolumeControl 

Enumeration Case

# LFEVolumeControl

The identifier for the low-frequency effect volume control class.

DriverKit 21.0+

``` source
LFEVolumeControl
```

## Discussion

This class is a subclass of the IOUserAudioLevelControl class for an LFE channel that results from bass management. If you use normal audio channels to represent LFE channels, you must use the VolumeControl class to manipulate the level.

## See Also

### Level and Volume Control Objects

LevelControl

The identifier for the audio level control class.

VolumeControl

The identifier for the audio volume control class.

