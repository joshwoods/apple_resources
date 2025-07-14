

- Force Feedback
- FFCUSTOMFORCE
-  rglForceData 

Instance Property

# rglForceData

Pointer to an array of force values representing the custom force. If multiple channels are provided, the values are interleaved. For example, if **cChannels** is 3, the first element of the array belongs to the first channel, the second to the second, and the third to the third.

Mac Catalyst 13.0+macOS 10.2+

``` source
var rglForceData: LPLONG!
```

## See Also

### Instance Properties

var cChannels: DWORD

Number of channels (axes) affected by this force.

var cSamples: DWORD

Total number of samples in the **rglForceData**. It must be an integral multiple of the **cChannels**.

var dwSamplePeriod: DWORD

Sample period, in microseconds.

