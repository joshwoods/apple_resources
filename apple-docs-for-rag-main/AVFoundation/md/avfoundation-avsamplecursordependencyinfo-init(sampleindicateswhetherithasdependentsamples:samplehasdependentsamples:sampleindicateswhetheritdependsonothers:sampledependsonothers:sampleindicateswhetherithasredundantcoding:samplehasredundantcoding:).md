

- AVFoundation
- AVSampleCursorDependencyInfo
-  init(sampleIndicatesWhetherItHasDependentSamples:sampleHasDependentSamples:sampleIndicatesWhetherItDependsOnOthers:sampleDependsOnOthers:sampleIndicatesWhetherItHasRedundantCoding:sampleHasRedundantCoding:) 

Initializer

# init(sampleIndicatesWhetherItHasDependentSamples:sampleHasDependentSamples:sampleIndicatesWhetherItDependsOnOthers:sampleDependsOnOthers:sampleIndicatesWhetherItHasRedundantCoding:sampleHasRedundantCoding:)

Creates a sample cursor dependency information structure with sample information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    sampleIndicatesWhetherItHasDependentSamples: ObjCBool,
    sampleHasDependentSamples: ObjCBool,
    sampleIndicatesWhetherItDependsOnOthers: ObjCBool,
    sampleDependsOnOthers: ObjCBool,
    sampleIndicatesWhetherItHasRedundantCoding: ObjCBool,
    sampleHasRedundantCoding: ObjCBool
)
```

## Parameters 

`sampleIndicatesWhetherItHasDependentSamples`  

A Boolean value that determines whether the sample indicates if other samples depend on it.

`sampleHasDependentSamples`  

A Boolean value that determines whether the sample has dependent samples.

`sampleIndicatesWhetherItDependsOnOthers`  

A Boolean value that determines whether the sample indicates that it depends on other samples.

`sampleDependsOnOthers`  

A Boolean value that determines whether the sample depends on other samples.

`sampleIndicatesWhetherItHasRedundantCoding`  

A Boolean value that determines whether the sample indicates that it has redundant coding.

`sampleHasRedundantCoding`  

A Boolean value that determines whether the sample has redundant coding.

