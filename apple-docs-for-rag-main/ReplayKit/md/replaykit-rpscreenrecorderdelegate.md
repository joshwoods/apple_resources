

- ReplayKit
-  RPScreenRecorderDelegate 

Protocol

# RPScreenRecorderDelegate

The protocol you implement to receive notifications from the screen recorder.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
protocol RPScreenRecorderDelegate : NSObjectProtocol
```

## Overview

Use this class to respond to changes to the screen recorder, represented by an RPScreenRecorder object.

## Topics

### Responding to Recording Changes

func screenRecorder(RPScreenRecorder, didStopRecordingWith: RPPreviewViewController?, error: (any Error)?)

Indicates that the screen recording has stopped.

func screenRecorderDidChangeAvailability(RPScreenRecorder)

Indicates that the recorder has changed states between disabled and enabled.

**Required**

func screenRecorder(RPScreenRecorder, didStopRecordingWithError: any Error, previewViewController: RPPreviewViewController?)

Indicates that the screen recording has stopped.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Inspecting a Screen Recorder

var isAvailable: Bool

A Boolean value that indicates whether the screen recorder is available for recording.

var isRecording: Bool

A Boolean value that indicates whether the app is currently recording.

var isMicrophoneEnabled: Bool

A Boolean value that indicates whether the microphone is currently enabled.

var isCameraEnabled: Bool

A Boolean value that indicates whether the camera is currently enabled.

var cameraPreviewView: UIView?

A view containing the contents of the front-facing camera.

var cameraPosition: RPCameraPosition

The camera position to use.

enum RPCameraPosition

The position of the camera being accessed.

var delegate: (any RPScreenRecorderDelegate)?

The delegate for the screen recorder.

