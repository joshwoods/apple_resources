

- MediaExtension
- MEHEVCDependencyInfo
-  syncSampleNALUnitType 

Instance Property

# syncSampleNALUnitType

The NAL unit type for HEVC sync sample groups.

macOS 14.0+

``` source
var syncSampleNALUnitType: Int16 { get set }
```

## Discussion

This value maps to the kCMSampleAttachmentKey_HEVCSyncSampleNALUnitType sample buffer attachment.

## See Also

### Inspecting the HEVC dependency attributes of a sample

var hasTemporalSubLayerAccess: Bool

A Boolean value that indicates if the sample has an HEVC temporal sublayer access (TSA) picture.

var hasStepwiseTemporalSubLayerAccess: Bool

A Boolean value that indicates if the sample has an HEVC stepwise temporal sublayer access (STSA) picture.

var temporalLevel: Int16

The HEVC temporal level, if available.

var profileSpace: Int16

The HEVC profile space, if available.

var tierFlag: Int16

The HEVC tier level flag, if available.

var profileIndex: Int16

The HEVC profile index, if available.

var profileCompatibilityFlags: Data?

The HEVC profile compatibility flags (4 bytes), if available.

var constraintIndicatorFlags: Data?

The HEVC constraint indicator flags (6 bytes), if available.

var levelIndex: Int16

The HEVC level index, if available.

