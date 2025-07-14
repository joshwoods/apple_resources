

- VisionKit
- ImageAnalysis
-  hasResults(for:) 

Instance Method

# hasResults(for:)

Returns a Boolean value that indicates whether the analysis finds the specified types in the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
final func hasResults(for analysisTypes: ImageAnalyzer.AnalysisTypes) -> Bool
```

## Parameters 

`analysisTypes`  

The data types you want to find in the image.

## Return Value

`true` if the image analysis has results for the specified types; otherwise, `false`.

