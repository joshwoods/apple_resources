

- Force Feedback
- FFCUSTOMFORCE
-  cChannels 

Instance Property

# cChannels

Number of channels (axes) affected by this force.

Mac Catalyst 13.0+macOS 10.2+

``` source
var cChannels: DWORD
```

## Discussion

The first channel is applied to the first axis associated with the effect, the second to the second, and so on. If there are fewer channels than axes, nothing is associated with the extra axes.

If there is only a single channel, the effect is rotated in the direction specified by the rglDirection member of the FFEFFECT structure. If there is more than one channel, rotation is not allowed.

Not all devices support rotation of custom effects.

## See Also

### Instance Properties

var cSamples: DWORD

Total number of samples in the **rglForceData**. It must be an integral multiple of the **cChannels**.

var dwSamplePeriod: DWORD

Sample period, in microseconds.

var rglForceData: LPLONG!

Pointer to an array of force values representing the custom force. If multiple channels are provided, the values are interleaved. For example, if **cChannels** is 3, the first element of the array belongs to the first channel, the second to the second, and the third to the third.

