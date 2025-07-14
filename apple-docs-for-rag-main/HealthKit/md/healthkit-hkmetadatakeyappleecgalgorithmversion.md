

- HealthKit
-  HKMetadataKeyAppleECGAlgorithmVersion 

Global Variable

# HKMetadataKeyAppleECGAlgorithmVersion

A key for metadata indicating the version number of the algorithm Apple Watch uses to generate an ECG reading.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
let HKMetadataKeyAppleECGAlgorithmVersion: String
```

## Discussion

Apple Watch sets this key on the HKElectrocardiogram samples it creates. The key is read-only.

## See Also

### Specifying Metadata

enum HKAppleECGAlgorithmVersion

Version numbers for the algorithm Apple Watch uses to generate an ECG reading.

