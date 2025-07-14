

- AVFoundation
- AVSampleCursorAudioDependencyInfo
-  audioSampleIsIndependentlyDecodable 

Instance Property

# audioSampleIsIndependentlyDecodable

A Boolean value indicating whether the sample is independently decodable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var audioSampleIsIndependentlyDecodable: ObjCBool
```

## Discussion

The value of this property is true for Immediate Playout Frames (IPFs) and Independent Frames (IFs).

## See Also

### Querying Independent Decodability

var audioSamplePacketRefreshCount: Int

The number of samples, starting at the current sample, that must be fed to the decoder to achieve full decoder refresh.

