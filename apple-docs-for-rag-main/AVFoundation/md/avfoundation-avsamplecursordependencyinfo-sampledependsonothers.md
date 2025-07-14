

- AVFoundation
- AVSampleCursorDependencyInfo
-  sampleDependsOnOthers 

Instance Property

# sampleDependsOnOthers

A Boolean value that determines whether the sample depends on other samples.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var sampleDependsOnOthers: ObjCBool
```

## Discussion

This value indicates whether the sample depends on other media samples when sampleIndicatesWhetherItDependsOnOthers is true.

## See Also

### Dependency Information

var sampleIndicatesWhetherItHasDependentSamples: ObjCBool

A Boolean value that determines whether the sample indicates if other samples depend on it.

var sampleHasDependentSamples: ObjCBool

A Boolean value that determines whether the sample has dependent samples.

var sampleIndicatesWhetherItDependsOnOthers: ObjCBool

A Boolean value that determines whether the sample indicates that it depends on other samples.

var sampleIndicatesWhetherItHasRedundantCoding: ObjCBool

A Boolean value that determines whether the sample indicates that it has redundant coding.

var sampleHasRedundantCoding: ObjCBool

A Boolean value that determines whether the sample has redundant coding.

