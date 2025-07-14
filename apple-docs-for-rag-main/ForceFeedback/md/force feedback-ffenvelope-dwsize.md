

- Force Feedback
- FFENVELOPE
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

var dwAttackLevel: DWORD

Amplitude for the start of the envelope, relative to the baseline, in the range from 0 through 10,000. If the effect’s type-specific data does not specify a baseline, the amplitude is relative to 0.

var dwAttackTime: DWORD

The time, in microseconds, to reach the sustain level.

var dwFadeLevel: DWORD

Amplitude for the end of the envelope, relative to the baseline, in the range from 0 through 10,000. If the effect’s type-specific data does not specify a baseline, the amplitude is relative to 0.

var dwFadeTime: DWORD

The time, in microseconds, to reach the fade level.

