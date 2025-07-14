

- Accelerate
-  vDSP_DFT_Setup 

Type Alias

# vDSP_DFT_Setup

An opaque type that contains setup information for a single-precision discrete Fourier transform (DFT).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias vDSP_DFT_Setup = OpaquePointer
```

## Discussion

Call the vDSP_DFT_zop_CreateSetup and vDSP_DFT_zrop_CreateSetup functions to initialize and allocate a new setup object. Call vDSP_DFT_DestroySetup to free the resources associated with a setup object.

## See Also

### Data types

typealias vDSP_DFT_Interleaved_Setup

An opaque type that contains setup information for an interleaved single-precision discrete Fourier transform (DFT).

typealias vDSP_DFT_Interleaved_SetupD

An opaque type that contains setup information for an interleaved double-precision discrete Fourier transform (DFT).

typealias vDSP_DFT_SetupD

An opaque type that contains setup information for a double-precision discrete Fourier transform (DFT).

