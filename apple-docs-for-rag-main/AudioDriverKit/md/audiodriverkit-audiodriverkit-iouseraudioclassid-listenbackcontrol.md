

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClassID
-  ListenbackControl 

Enumeration Case

# ListenbackControl

The identifier for the audio listenback control class.

DriverKit 21.0+

``` source
ListenbackControl
```

## Discussion

This class is a subclass of the IOUserAudioBooleanControl class where a `true` value indcates an enabled listenback channel. This control is for listenback channels outside of the regular I/O channels. If the listenback channel is among the normal I/O channels, it uses MuteControl.

## See Also

### Boolean Controls

BooleanControl

The identifier for the audio Boolean control class.

LFEMuteControl

The identifier for the low-frequency effect mute control class.

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

