

- MediaExtension
- MEHEVCDependencyInfo
-  tierFlag 

Instance Property

# tierFlag

The HEVC tier level flag, if available.

macOS 14.0+

``` source
var tierFlag: Int16 { get set }
```

## Discussion

This value maps to the kCMHEVCTemporalLevelInfoKey_TierFlag sample buffer attachment, and is `-1` if this information isn’t available.

## See Also

### Inspecting the HEVC dependency attributes of a sample

var hasTemporalSubLayerAccess: Bool

A Boolean value that indicates if the sample has an HEVC temporal sublayer access (TSA) picture.

var hasStepwiseTemporalSubLayerAccess: Bool

A Boolean value that indicates if the sample has an HEVC stepwise temporal sublayer access (STSA) picture.

var syncSampleNALUnitType: Int16

The NAL unit type for HEVC sync sample groups.

var temporalLevel: Int16

The HEVC temporal level, if available.

var profileSpace: Int16

The HEVC profile space, if available.

var profileIndex: Int16

The HEVC profile index, if available.

var profileCompatibilityFlags: Data?

The HEVC profile compatibility flags (4 bytes), if available.

var constraintIndicatorFlags: Data?

The HEVC constraint indicator flags (6 bytes), if available.

var levelIndex: Int16

The HEVC level index, if available.

