

- SensitiveContentAnalysis
- SCSensitivityAnalysis
-  isSensitive 

Instance Property

# isSensitive

A Boolean value that indicates if checked content contains nudity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
var isSensitive: Bool { get }
```

## Mentioned in 

Testing your app’s response to sensitive media

## Discussion

The framework indicates that content is sensitive only when the active analysisPolicy is a value other than SCSensitivityAnalysisPolicy.disabled.

