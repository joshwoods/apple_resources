

- SensitiveContentAnalysis
- SCSensitivityAnalyzer
-  videoAnalysis(forFileAt:) 

Instance Method

# videoAnalysis(forFileAt:)

Analyzes a video file on disk at a URL for sensitive content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
func videoAnalysis(forFileAt fileURL: URL) -> SCSensitivityAnalyzer.VideoAnalysisHandler
```

## Parameters 

`fileURL`  

The URL for a video file on disk.

## Return Value

An object that checks if a video contains sensitive content and provides the app with status updates as the analysis progresses.

## See Also

### Analyzing video

class VideoAnalysisHandler

An object that checks if a video contains sensitive content and provides status updates.

