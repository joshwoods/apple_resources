

- ScreenCaptureKit
- SCStreamOutput
-  stream(\_:didOutputSampleBuffer:of:) 

Instance Method

# stream(\_:didOutputSampleBuffer:of:)

Tells the delegate that a capture stream produced a frame.

Mac Catalyst 18.2+macOS 12.3+

``` source
optional func stream(
    _ stream: SCStream,
    didOutputSampleBuffer sampleBuffer: CMSampleBuffer,
    of type: SCStreamOutputType
)
```

## Parameters 

`stream`  

The frame capture stream that produced this frame.

`sampleBuffer`  

The sample buffer containing capture data.

`type`  

The type of capture contained in the sample buffer.

