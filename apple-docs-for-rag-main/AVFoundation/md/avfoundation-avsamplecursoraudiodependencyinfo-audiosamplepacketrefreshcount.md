

- AVFoundation
- AVSampleCursorAudioDependencyInfo
-  audioSamplePacketRefreshCount 

Instance Property

# audioSamplePacketRefreshCount

The number of samples, starting at the current sample, that must be fed to the decoder to achieve full decoder refresh.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var audioSamplePacketRefreshCount: Int
```

## Discussion

The value of audioSampleIsIndependentlyDecodable must be true for this value to take effect.

The value of this property is `0` for Immediate Playout Frames (IPFs).

## See Also

### Querying Independent Decodability

var audioSampleIsIndependentlyDecodable: ObjCBool

A Boolean value indicating whether the sample is independently decodable.

