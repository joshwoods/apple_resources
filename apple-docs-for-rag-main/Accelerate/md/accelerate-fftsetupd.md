

- Accelerate
-  FFTSetupD 

Type Alias

# FFTSetupD

An opaque type that contains setup information for a double-precision FFT transform.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias FFTSetupD = OpaquePointer
```

## Discussion

Call the vDSP_create_fftsetupD function to create a setup structure, and calll vDSP_destroy_fftsetupD to deallocate a setup structure.

## See Also

### FFT Setup

typealias FFTSetup

An opaque type that contains setup information for a single-precision FFT transform.

typealias FFTRadix

The radix of the FFT decomposition.

