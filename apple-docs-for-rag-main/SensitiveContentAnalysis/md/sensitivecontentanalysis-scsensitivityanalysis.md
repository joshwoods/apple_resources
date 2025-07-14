

- SensitiveContentAnalysis
-  SCSensitivityAnalysis 

Class

# SCSensitivityAnalysis

An object that determines if checked content contains nudity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
class SCSensitivityAnalysis
```

## Mentioned in 

Testing your app’s response to sensitive media

## Overview

The completion handler for SCSensitivityAnalyzer methods, such as analyzeImage(_:completionHandler:), receive an instance of this type as a `results` parameter.

```
// Check a loaded image for nudity.
let response = try await analyzer.analyzeImage(image.cgImage)

if response.isSensitive {
    // Check the active `analysisPolicy` on how to proceed.
}
```

For more information about checking the active analysisPolicy, see SCSensitivityAnalysisPolicy.

## Topics

### Content-sensitivity check results

var isSensitive: Bool

A Boolean value that indicates if checked content contains nudity.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

