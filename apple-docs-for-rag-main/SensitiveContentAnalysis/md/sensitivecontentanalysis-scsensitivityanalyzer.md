

- SensitiveContentAnalysis
-  SCSensitivityAnalyzer 

Class

# SCSensitivityAnalyzer

An object that analyzes media for sensitive content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
class SCSensitivityAnalyzer
```

## Mentioned in 

Detecting nudity in media and providing intervention options

Testing your app’s response to sensitive media

## Overview

To check an image for nudity, call one of this class’s `analyzeImage` methods and pass in a user-provided image, or a URL to the image.

```
// Analyze an image file at a particular URL.
let response = try await analyzer.analyzeImage(at: url)
```

To analyze a video file, pass a URL to a video on disk into videoAnalysis(forFileAt:) and wait for the hasSensitiveContent() method to complete.

```
let handler = analyzer.videoAnalysis(forFileAt: videoFileUrl)
let response = try await handler.hasSensitiveContent()
```

This class successfully detects nudity only when analysisPolicy is a value other than SCSensitivityAnalysisPolicy.disabled.

## Topics

### Creating a sensitivity analyzer

init()

Creates a sensitivity analyzer.

### Determining a nudity detection strategy

var analysisPolicy: SCSensitivityAnalysisPolicy

A property that determines if the app detects nudity and how the app responds.

### Analyzing images

func analyzeImage(CGImage, completionHandler: (SCSensitivityAnalysis?, (any Error)?) -> Void)

Analyzes an image for sensitive content and runs code on completion.

func analyzeImage(at: URL, completionHandler: (SCSensitivityAnalysis?, (any Error)?) -> Void)

Analyzes an image file on disk at a URL and runs code on completion.

### Analyzing video

func videoAnalysis(forFileAt: URL) -> SCSensitivityAnalyzer.VideoAnalysisHandler

Analyzes a video file on disk at a URL for sensitive content.

class VideoAnalysisHandler

An object that checks if a video contains sensitive content and provides status updates.

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

## See Also

### Content analysis

enum SCSensitivityAnalysisPolicy

Configurations that represent the way the framework checks for sensitive content and how the app responds.

