

- Audio Toolbox
-  kConverterPrimeMethod_None 

Global Variable

# kConverterPrimeMethod_None

Acts in “latency” mode. Leading and trailing frames are both assumed to be silence.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kConverterPrimeMethod_None: UInt32 { get }
```

## See Also

### Constants

var kConverterPrimeMethod_Pre: UInt32

Prime with `leading` + `trailing` input frames.

var kConverterPrimeMethod_Normal: UInt32

Prime with `trailing` frames only, for zero latency. Leading frames are assumed to be silence.

