

- AudioDriverKit
- AudioDriverKit
- IOUserAudioClassID
-  ClipLightControl 

Enumeration Case

# ClipLightControl

The identifier for the audio clip light control class.

DriverKit 21.0+

``` source
ClipLightControl
```

## Discussion

This class is a subclass of the `IOUserAudioBooleanControl` class where a true value indcates the signal for the element has exceeded the sample range. After a clip light turns on, it stays on until either:

A `SetControlValue` call sets the value to `false`.

The current IO session stops and a new IO session starts.

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

TalkbackControl

The identifier for the audio talkback control class.

ListenbackControl

The identifier for the audio listenback control class.

