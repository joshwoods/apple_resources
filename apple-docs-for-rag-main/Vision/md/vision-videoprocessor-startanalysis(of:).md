

- Vision
- VideoProcessor
-  startAnalysis(of:) 

Instance Method

# startAnalysis(of:)

Begins analyzing video frames.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final func startAnalysis(of timeRange: CMTimeRange? = nil)
```

## Parameters 

`timeRange`  

The range of video timestamps to process.

## Discussion

By default the framework processes the entire video.

