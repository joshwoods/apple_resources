

- SensitiveContentAnalysis
- SCSensitivityAnalyzer
-  SCSensitivityAnalyzer.VideoAnalysisHandler 

Class

# SCSensitivityAnalyzer.VideoAnalysisHandler

An object that checks if a video contains sensitive content and provides status updates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
final class VideoAnalysisHandler
```

## Overview

Checking video for sensitive content can take longer than checking images. This class enables an app to stay informed on the framework’s progress while it checks a video for sensitive content. The SCSensitivityAnalyzer method videoAnalysis(forFileAt:) returns an instance of this class.

To analyze a video file for sensitive content, pass a video URL into the videoAnalysis(forFileAt:) function. While waiting on the hasSensitiveContent() method, check progress for the completion status:

```
let handler = analyzer.videoAnalysis(forFileAt: videoFileUrl)

let progress = handler.progress
// Do something with the `progress` property, such as dispatch a UI update thread.

// Wait here until the video check for sensitive content completes.
let response = try await handler.hasSensitiveContent()
```

## Topics

### Checking progress

var progress: Progress

An object that provides the app with status updates while a sensitive content check occurs for a video.

### Determining sensitivity

func hasSensitiveContent() async throws -> SCSensitivityAnalysis

Provides a result that indicates if the video file contains sensitive content.

## See Also

### Analyzing video

func videoAnalysis(forFileAt: URL) -> SCSensitivityAnalyzer.VideoAnalysisHandler

Analyzes a video file on disk at a URL for sensitive content.

