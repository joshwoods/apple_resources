

- Force Feedback
- FFEFFECT
-  dwSize 

Instance Property

# dwSize

Size, in bytes, of this structure. This member must be initialized before the structure is used.

Mac Catalyst 13.0+macOS 10.2+

``` source
var dwSize: DWORD
```

## See Also

### Instance Properties

var cAxes: DWORD

Number of axes involved in the effect.

var cbTypeSpecificParams: DWORD

Number of bytes of additional type-specific parameters for the corresponding effect type.

var dwDuration: DWORD

The total duration of the effect, in microseconds. If this value is FF_INFINITE, the effect has infinite duration. If an envelope has been applied to the effect, the attack is applied, followed by an infinite sustain.

var dwFlags: DWORD

Flags associated with an effect.

var dwGain: DWORD

The gain to be applied to the effect, in the range from 0 through 10,000. The gain is a scaling factor applied to all magnitudes of the effect and its envelope.

var dwSamplePeriod: DWORD

The period at which the device should play back the effect, in microseconds.

var dwStartDelay: DWORD

Time (in microseconds) that the device should wait after a FFEffectStart call before playing the effect. If this value is 0, effect playback begins immediately.

var dwTriggerButton: DWORD

The identifier or offset of the button to be used to trigger playback of the effect. The FFJOFS\_\* flags must be used to specify the value. If this member is set to FFEB_NOTRIGGER, no trigger button is associated with the effect.

var dwTriggerRepeatInterval: DWORD

The interval, in microseconds, between the end of one playback and the start of the next when the effect is triggered by a button press and the button is held down. Setting this value to FF_INFINITE suppresses repetition.

var lpEnvelope: PFFENVELOPE!

Optional pointer to a FFENVELOPE structure that describes the envelope to be used by this effect. Not all effect types use envelopes. If no envelope is to be applied, the member should be set to NULL.

var lpvTypeSpecificParams: UnsafeMutableRawPointer!

A pointer to type-specific parameters, or NULL if there are no type-specific parameters.

var rgdwAxes: LPDWORD!

Pointer to a DWORD array (of **cAxes** elements) containing identifiers or offsets identifying the axes to which the effect is to be applied.

var rglDirection: LPLONG!

Pointer to a LONG array (of **cAxes** elements) containing either Cartesian coordinates, polar coordinates, or spherical coordinates.

