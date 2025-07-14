

- AVFoundation
- AVCaptureAudioDataOutputSampleBufferDelegate
-  captureOutput(\_:didOutput:from:) 

Instance Method

# captureOutput(\_:didOutput:from:)

Notifies the delegate that a sample buffer was written.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
optional func captureOutput(
    _ output: AVCaptureOutput,
    didOutput sampleBuffer: CMSampleBuffer,
    from connection: AVCaptureConnection
)
```

## Parameters 

`output`  

The capture output object.

`sampleBuffer`  

The sample buffer that was output.

`connection`  

The connection.

