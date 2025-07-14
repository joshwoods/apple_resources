

- AVFoundation
- AVCaptureVideoDataOutputSampleBufferDelegate
-  captureOutput(\_:didDrop:from:) 

Instance Method

# captureOutput(\_:didDrop:from:)

Notifies the delegate that a video frame was discarded.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
optional func captureOutput(
    _ output: AVCaptureOutput,
    didDrop sampleBuffer: CMSampleBuffer,
    from connection: AVCaptureConnection
)
```

## Parameters 

`output`  

The capture output object.

`sampleBuffer`  

A `CMSampleBuffer` object containing information about the dropped frame, such as its format and presentation time.

This sample buffer contains none of the original video data.

`connection`  

The connection from which the video was received.

## Discussion

Delegates receive this message whenever a late video frame is dropped. This method is called once for each dropped frame. It is called on the dispatch queue specified by the output’s sampleBufferCallbackQueue property.

The `sampleBuffer` will contain a kCMSampleBufferAttachmentKey_DroppedFrameReason attachment that details why the frame was dropped. The frame may be dropped because it was late (kCMSampleBufferDroppedFrameReason_FrameWasLate), typically caused by the client’s processing taking too long. It can also be dropped because the module providing frames is out of buffers (kCMSampleBufferDroppedFrameReason_OutOfBuffers). Frames can also be dropped if the module providing sample buffers has experienced a discontinuity (kCMSampleBufferDroppedFrameReason_Discontinuity) and an unknown number of frames have been lost. This condition is typically caused by the system being too busy.

Because this method is called on the same dispatch queue that is responsible for outputting video frames, it must be efficient to prevent further capture performance problems, such as additional dropped video frames.

## See Also

### Managing Sample Buffer Behavior

func captureOutput(AVCaptureOutput, didOutput: CMSampleBuffer, from: AVCaptureConnection)

Notifies the delegate that a new video frame was written.

