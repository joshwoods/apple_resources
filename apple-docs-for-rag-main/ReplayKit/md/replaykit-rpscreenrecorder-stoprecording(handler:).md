

- ReplayKit
- RPScreenRecorder
-  stopRecording(handler:) 

Instance Method

# stopRecording(handler:)

Stops the current recording.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func stopRecording(handler: ((RPPreviewViewController?, (any Error)?) -> Void)? = nil)
```

## Parameters 

`handler`  

A block that is called when the request completes.

`previewViewController`  
An instance of the `RPPreviewViewController` class.

`error`  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes to ReplayKit.

## Discussion

When recording stops with no associated error, present the resulting preview view controller using present(_:animated:completion:). The user will see the built-in preview view controller with options to trim, cut, and share the recording. On iPad, you must present the preview view controller as a popover.

Listing 1. Presenting the preview view controller on iPad

```
sharedRecorder.stopRecording { previewViewController, error in
    guard let _ = error else {
        print("\(error?.localizedDescription ?? "Error")")
        return
    }
    if let previewViewController = previewViewController {
        if UIDevice.current.userInterfaceIdiom == .pad {
            previewViewController.modalPresentationStyle = .popover
            previewViewController.popoverPresentationController?.sourceRect = .zero
            previewViewController.popoverPresentationController?.sourceView = self.view
        }

        self.previewViewController = previewViewController
        previewViewController.previewControllerDelegate = self

        // Present the view controller.
        self.present(previewViewController, animated: true, completion: nil)
    }
}
```

## See Also

### Controlling App Recording

func startRecording(handler: (((any Error)?) -> Void)?)

Starts recording the app display.

func stopRecording(withOutput: URL, completionHandler: (((any Error)?) -> Void)?)

Stops the current recording and writes the movie to the specified output URL.

func startCapture(handler: ((CMSampleBuffer, RPSampleBufferType, (any Error)?) -> Void)?, completionHandler: (((any Error)?) -> Void)?)

Starts screen and audio capture.

enum RPSampleBufferType

The type of media clip sample being buffered.

func stopCapture(handler: (((any Error)?) -> Void)?)

Stops screen capture

func discardRecording(handler: () -> Void)

Discards the current recording.

func startRecording(withMicrophoneEnabled: Bool, handler: (((any Error)?) -> Void)?)

Starts recording the app’s audio and video.

Deprecated

