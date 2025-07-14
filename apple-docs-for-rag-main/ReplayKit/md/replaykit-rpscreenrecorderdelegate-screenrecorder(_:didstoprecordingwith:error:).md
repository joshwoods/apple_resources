

- ReplayKit
- RPScreenRecorderDelegate
-  screenRecorder(\_:didStopRecordingWith:error:) 

Instance Method

# screenRecorder(\_:didStopRecordingWith:error:)

Indicates that the screen recording has stopped.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
optional func screenRecorder(
    _ screenRecorder: RPScreenRecorder,
    didStopRecordingWith previewViewController: RPPreviewViewController?,
    error: (any Error)?
)
```

## Parameters 

`screenRecorder`  

The RPScreenRecorder instance.

`previewViewController`  

An RPPreviewViewController interface object that is returned if anything at all was recorded. The interface allows the user to preview and edit the recording.

`error`  

An NSError describing why the recording stopped. This method is `nil` when no error occurs.

## Discussion

This method is called when recording stops due to an error or a change in recording availability. If any part of the stopped recording is available, an instance of RPPreviewViewController is returned.

## See Also

### Responding to Recording Changes

func screenRecorderDidChangeAvailability(RPScreenRecorder)

Indicates that the recorder has changed states between disabled and enabled.

**Required**

func screenRecorder(RPScreenRecorder, didStopRecordingWithError: any Error, previewViewController: RPPreviewViewController?)

Indicates that the screen recording has stopped.

Deprecated

