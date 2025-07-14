

- AVFoundation
- AVCaptureSession
-  canAddOutput(\_:) 

Instance Method

# canAddOutput(\_:)

Determines whether you can add an output to a session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func canAddOutput(_ output: AVCaptureOutput) -> Bool
```

## Parameters 

`output`  

An output to add to the session.

## Return Value

true if you can add the output; otherwise false.

## Discussion

In iOS and Mac Catalyst, the system imposes the following limitations on the combinations of outputs a capture session may contain:

- An app may add only a single output of a particular type. For apps that link against iOS 16 or later, this restriction no longer applies to AVCaptureVideoDataOutput.

- Prior to iOS 16, you can add an AVCaptureVideoDataOutput and an AVCaptureMovieFileOutput to the same session, but only one may have its connection active. If you attempt to enable both connections, the system chooses the movie file output as the active connection and disables the video data output’s connection. For apps that link against iOS 16 or later, this restriction no longer exists.

- Similarly, prior to iOS 16, you can add an AVCaptureAudioDataOutput and an AVCaptureMovieFileOutput to the same session, but only one may have its connection active. If you attempt to enable both connections, the system chooses the movie file output and disables the audio data output’s connection. For apps that link against iOS 16 or later, this restriction no longer exists.

- An app can’t add an AVCapturePhotoOutput and AVCaptureStillImageOutput to the same session.

Important

If you configure a capture session to use more than one AVCaptureVideoDataOutput instance, monitor the value of the capture session’s hardwareCost property and reconfigure the session as appropriate.

## See Also

### Configuring Outputs

var outputs: [AVCaptureOutput]

The output destinations to which a captures session sends its data.

func addOutput(AVCaptureOutput)

Adds an output to the capture session.

func removeOutput(AVCaptureOutput)

Removes an output from a capture session.

