

- AVFoundation
- AVCaptureFileOutputDelegate
-  fileOutputShouldProvideSampleAccurateRecordingStart(\_:) 

Instance Method

# fileOutputShouldProvideSampleAccurateRecordingStart(\_:)

Allows a client to opt in to frame accurate recording in fileOutput(_:didOutputSampleBuffer:from:).

macOS 10.8+

``` source
func fileOutputShouldProvideSampleAccurateRecordingStart(_ output: AVCaptureFileOutput) -> Bool
```

**Required**

## Parameters 

`output`  

The capture file output instance that is associated with the delegate.

## Return Value

true if frame accurate recording is required; otherwise false.

## Discussion

In apps linked before OS X Mountain Lion, delegates that implement the fileOutput(_:didOutputSampleBuffer:from:) method can ensure that starting and stopping a recording is frame accurate by calling startRecording(to:recordingDelegate:) or stopRecording() from within the callback. Frame accurate recording requires the capture output to apply outputSettings when the session starts running, so it is ready to start and/or stop recording on any given frame boundary. Applying compression settings for the entire length of the session has power, thermal, and CPU implications.

In apps linked on or after OS X Mountain Lion, delegates must implement this method to indicate whether frame accurate recording is required. The capture file output calls this method only once when the delegate is added and never again. If your delegate returns false, the capture file output applies compression settings only when startRecording(to:recordingDelegate:) is called and disables these settings once the recording stops.

## See Also

### Sample Processing

func fileOutput(AVCaptureFileOutput, didOutputSampleBuffer: CMSampleBuffer, from: AVCaptureConnection)

Gives the delegate the opportunity to inspect samples as they are received by the output and start and stop recording at exact times.

