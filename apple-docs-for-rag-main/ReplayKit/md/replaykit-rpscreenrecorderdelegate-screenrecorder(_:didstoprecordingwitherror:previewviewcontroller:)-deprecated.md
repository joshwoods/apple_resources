

- ReplayKit
- RPScreenRecorderDelegate
-  screenRecorder(\_:didStopRecordingWithError:previewViewController:) Deprecated

Instance Method

# screenRecorder(\_:didStopRecordingWithError:previewViewController:)

Indicates that the screen recording has stopped.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–10.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func screenRecorder(
    _ screenRecorder: RPScreenRecorder,
    didStopRecordingWithError error: any Error,
    previewViewController: RPPreviewViewController?
)
```

Deprecated

No longer supported

## Parameters 

`screenRecorder`  

The RPScreenRecorder instance.

`error`  

An NSError describing why the recording stopped.

`previewViewController`  

An RPPreviewViewController interface object that is returned if anything at all was recorded. The interface allows the user to preview and edit the recording.

## Discussion

screenRecorder(_:didStopRecordingWithError:previewViewController:) is called when recording stops due to an error or a change in recording availability. If any part of the stopped recording is available, an instance of RPPreviewViewController is returned.

## See Also

### Responding to Recording Changes

func screenRecorder(RPScreenRecorder, didStopRecordingWith: RPPreviewViewController?, error: (any Error)?)

Indicates that the screen recording has stopped.

func screenRecorderDidChangeAvailability(RPScreenRecorder)

Indicates that the recorder has changed states between disabled and enabled.

**Required**

