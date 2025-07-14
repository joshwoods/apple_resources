

- HealthKit
-  HKAppleECGAlgorithmVersion 

Enumeration

# HKAppleECGAlgorithmVersion

Version numbers for the algorithm Apple Watch uses to generate an ECG reading.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
enum HKAppleECGAlgorithmVersion
```

## Topics

### Versions

case version1

The version 1 algorithm.

case version2

The version 2 algorithm.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Metadata

let HKMetadataKeyAppleECGAlgorithmVersion: String

A key for metadata indicating the version number of the algorithm Apple Watch uses to generate an ECG reading.

