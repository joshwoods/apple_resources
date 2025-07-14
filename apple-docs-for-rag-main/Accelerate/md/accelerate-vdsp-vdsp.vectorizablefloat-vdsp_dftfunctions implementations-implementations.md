

- Accelerate
- vDSP
- vDSP.VectorizableFloat
-  vDSP_DFTFunctions Implementations 

API Collection

# vDSP_DFTFunctions Implementations

## Topics

### Type Methods

static func destroySetup(OpaquePointer)Deprecated

static func makeDFTSetup&lt;T>(previous: vDSP.DFT&lt;T>?, count: Int, direction: vDSP.FourierTransformDirection, transformType: vDSP.DFTTransformType) -> OpaquePointer?Deprecated

static func transform&lt;U, V>(dftSetup: OpaquePointer, inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)Deprecated

