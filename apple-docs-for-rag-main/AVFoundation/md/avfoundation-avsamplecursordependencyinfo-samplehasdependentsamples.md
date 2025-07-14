

- AVFoundation
- AVSampleCursorDependencyInfo
-  sampleHasDependentSamples 

Instance Property

# sampleHasDependentSamples

A Boolean value that determines whether the sample has dependent samples.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var sampleHasDependentSamples: ObjCBool
```

## Discussion

This value indicates the sample has dependent samples when sampleIndicatesWhetherItHasDependentSamples is true.

## See Also

### Dependency Information

var sampleIndicatesWhetherItHasDependentSamples: ObjCBool

A Boolean value that determines whether the sample indicates if other samples depend on it.

var sampleIndicatesWhetherItDependsOnOthers: ObjCBool

A Boolean value that determines whether the sample indicates that it depends on other samples.

var sampleDependsOnOthers: ObjCBool

A Boolean value that determines whether the sample depends on other samples.

var sampleIndicatesWhetherItHasRedundantCoding: ObjCBool

A Boolean value that determines whether the sample indicates that it has redundant coding.

var sampleHasRedundantCoding: ObjCBool

A Boolean value that determines whether the sample has redundant coding.

