

- Force Feedback
- FFCUSTOMFORCE
-  dwSamplePeriod 

Instance Property

# dwSamplePeriod

Sample period, in microseconds.

Mac Catalyst 13.0+macOS 10.2+

``` source
var dwSamplePeriod: DWORD
```

## See Also

### Instance Properties

var cChannels: DWORD

Number of channels (axes) affected by this force.

var cSamples: DWORD

Total number of samples in the **rglForceData**. It must be an integral multiple of the **cChannels**.

var rglForceData: LPLONG!

Pointer to an array of force values representing the custom force. If multiple channels are provided, the values are interleaved. For example, if **cChannels** is 3, the first element of the array belongs to the first channel, the second to the second, and the third to the third.

