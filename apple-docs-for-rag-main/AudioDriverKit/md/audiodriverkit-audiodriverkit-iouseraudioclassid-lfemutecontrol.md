

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClassID
-  LFEMuteControl 

Enumeration Case

# LFEMuteControl

The identifier for the low-frequency effect mute control class.

DriverKit 21.0+

``` source
LFEMuteControl
```

## Discussion

This class is a subclass of the IOUserAudioBooleanControl class, where `true` means that the LFE channel that results from bass management isn’t audible. If you use normal audio channels to represent LFE channels, you must use the VolumeControl class to manipulate the level.

## See Also

### Boolean Controls

BooleanControl

The identifier for the audio Boolean control class.

SoloControl

The identifier for the audio solo control class.

JackControl

The identifier for the audio jack control class.

PhantomPowerControl

The identifier for the audio phantom power control class.

PhaseInvertControl

The identifier for the audio phase invert control class.

ClipLightControl

The identifier for the audio clip light control class.

TalkbackControl

The identifier for the audio talkback control class.

ListenbackControl

The identifier for the audio listenback control class.

