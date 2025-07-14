

- Accelerate
- vDSP
- vDSP.VectorizableDouble
-  vDSP_BiquadFunctions Implementations 

API Collection

# vDSP_BiquadFunctions Implementations

## Topics

### Type Methods

static func applyMulti(setup: vDSP_biquadm_SetupD, pInputs: UnsafeMutablePointer&lt;UnsafePointer&lt;vDSP.VectorizableDouble.Scalar>>, pOutputs: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;vDSP.VectorizableDouble.Scalar>>, count: vDSP_Length)

static func applySingle&lt;U, V>(source: U, destination: inout V, delays: UnsafeMutablePointer&lt;vDSP.VectorizableDouble.Scalar>, setup: vDSP_biquad_Setup, sectionCount: vDSP_Length, count: vDSP_Length)

static func destroySetup(channelCount: UInt, biquadSetup: OpaquePointer)

static func makeBiquadSetup(channelCount: vDSP_Length, coefficients: [Double], sectionCount: vDSP_Length) -> OpaquePointer?

