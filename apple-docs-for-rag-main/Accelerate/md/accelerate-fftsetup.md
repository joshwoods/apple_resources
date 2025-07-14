

- Accelerate
-  FFTSetup 

Type Alias

# FFTSetup

An opaque type that contains setup information for a single-precision FFT transform.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias FFTSetup = OpaquePointer
```

## Discussion

Call the vDSP_create_fftsetup function to create a setup structure, and calll vDSP_destroy_fftsetup to deallocate a setup structure.

## See Also

### FFT Setup

typealias FFTSetupD

An opaque type that contains setup information for a double-precision FFT transform.

typealias FFTRadix

The radix of the FFT decomposition.

