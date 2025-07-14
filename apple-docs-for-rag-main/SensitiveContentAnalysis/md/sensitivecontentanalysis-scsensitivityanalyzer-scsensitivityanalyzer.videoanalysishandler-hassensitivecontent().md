

- SensitiveContentAnalysis
- SCSensitivityAnalyzer
- SCSensitivityAnalyzer.VideoAnalysisHandler
-  hasSensitiveContent() 

Instance Method

# hasSensitiveContent()

Provides a result that indicates if the video file contains sensitive content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
final func hasSensitiveContent() async throws -> SCSensitivityAnalysis
```

## Return Value

An object that indicates if checked content contains nudity.

