

- Accelerate
-  vDSP_BiquadFunctions 

Protocol

# vDSP_BiquadFunctions

A protocol that defines functions for biquadratic filtering.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
protocol vDSP_BiquadFunctions
```

## Topics

### Associated Types

associatedtype Scalar

**Required**

### Type Methods

static func applyMulti(setup: vDSP_biquadm_SetupD, pInputs: UnsafeMutablePointer&lt;UnsafePointer&lt;Self.Scalar>>, pOutputs: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;Self.Scalar>>, count: vDSP_Length)

**Required**

static func applySingle&lt;U, V>(source: U, destination: inout V, delays: UnsafeMutablePointer&lt;Self.Scalar>, setup: vDSP_biquad_Setup, sectionCount: vDSP_Length, count: vDSP_Length)

**Required**

static func destroySetup(channelCount: UInt, biquadSetup: OpaquePointer)

**Required**

static func makeBiquadSetup(channelCount: vDSP_Length, coefficients: [Double], sectionCount: vDSP_Length) -> OpaquePointer?

**Required**

## Relationships

### Conforming Types

- vDSP.VectorizableDouble
- vDSP.VectorizableFloat

## See Also

### Biquadratic Filtering

protocol vDSP_FloatingPointBiquadFilterable

Types that support biquadratic filtering.

