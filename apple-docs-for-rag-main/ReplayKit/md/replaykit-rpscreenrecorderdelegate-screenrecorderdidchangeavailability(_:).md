

- ReplayKit
- RPScreenRecorderDelegate
-  screenRecorderDidChangeAvailability(\_:) 

Instance Method

# screenRecorderDidChangeAvailability(\_:)

Indicates that the recorder has changed states between disabled and enabled.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
optional func screenRecorderDidChangeAvailability(_ screenRecorder: RPScreenRecorder)
```

**Required**

## Parameters 

`screenRecorder`  

The RPScreenRecorder instance that has changed state.

## Discussion

Screen recording can be unavailable due to unsupported hardware, the user’s device displaying information over Airplay or through a TVOut session, or another app using the shared recorder.

## See Also

### Responding to Recording Changes

func screenRecorder(RPScreenRecorder, didStopRecordingWith: RPPreviewViewController?, error: (any Error)?)

Indicates that the screen recording has stopped.

func screenRecorder(RPScreenRecorder, didStopRecordingWithError: any Error, previewViewController: RPPreviewViewController?)

Indicates that the screen recording has stopped.

Deprecated

