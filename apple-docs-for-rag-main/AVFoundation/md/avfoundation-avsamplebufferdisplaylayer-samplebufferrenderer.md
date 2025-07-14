

- AVFoundation
- AVSampleBufferDisplayLayer
-  sampleBufferRenderer 

Instance Property

# sampleBufferRenderer

An object that enqueues video sample buffers for rendering.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var sampleBufferRenderer: AVSampleBufferVideoRenderer { get }
```

## Discussion

This object allows you to safely enqueue sample buffers from a background thread.

