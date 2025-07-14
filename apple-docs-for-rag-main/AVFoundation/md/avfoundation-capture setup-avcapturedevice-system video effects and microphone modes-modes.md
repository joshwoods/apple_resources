

- AVFoundation
- Capture setup
- AVCaptureDevice
-  System Video Effects and Microphone Modes 

API Collection

# System Video Effects and Microphone Modes

Configure the state of system video effects like Center Stage, and inspect enhancements the system applies to microphone audio.

## Topics

### Performing Reaction Effects

class var reactionEffectsEnabled: Bool

A Boolean value that indicates whether the app supports performing reaction effects.

var canPerformReactionEffects: Bool

A Boolean value that indicates whether you can perform reaction effects on a capture device.

var availableReactionTypes: Set&lt;AVCaptureReactionType>

A set of reactions types that a device supports performing.

class var reactionEffectGesturesEnabled: Bool

A Boolean value that indicates whether gesture detection triggers reaction effects on the video stream.

func performEffect(for: AVCaptureReactionType)

Performs the specified reaction type on the video stream.

var reactionEffectsInProgress: [AVCaptureReactionEffectState]

An array of reaction effects that the device is currently performing, sorted by timestamp.

class AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

### Configuring Center Stage

var isCenterStageActive: Bool

A Boolean value that indicates whether Center Stage is active on a device.

class var isCenterStageEnabled: Bool

A Boolean value that indicates whether a user or an app enabled Center Stage on a device.

var centerStageRectOfInterest: CGRect

The effective region within the output pixel buffer to perform Center Stage framing.

class var centerStageControlMode: AVCaptureDevice.CenterStageControlMode

A value that indicates the current mode of Center Stage control.

enum CenterStageControlMode

Constants that indicate the current Center Stage control mode.

### Configuring Studio Light

var isStudioLightActive: Bool

A Boolean value that indicates whether Studio Light is active on a device.

class var isStudioLightEnabled: Bool

A Boolean value that indicates whether a user enabled Studio Light on a device.

### Inspecting the Portrait Effect Settings

var isPortraitEffectActive: Bool

A Boolean value that indicates whether the Portrait video effect is active on a device.

class var isPortraitEffectEnabled: Bool

A Boolean value that indicates whether the user enabled the Portrait video effect in Control Center.

### Inspecting the Microphone Mode

class var activeMicrophoneMode: AVCaptureDevice.MicrophoneMode

The device’s active microphone mode.

class var preferredMicrophoneMode: AVCaptureDevice.MicrophoneMode

The microphone mode that the user selects in Control Center.

enum MicrophoneMode

Constants that define the available microphone modes.

### Presenting the Configuration User Interface

class func showSystemUserInterface(AVCaptureDevice.SystemUserInterface)

Displays the system’s user interface to configure video effects or microphone modes.

enum SystemUserInterface

Constants that describe the capture device configuration user interfaces.

### Configuring Background Replacement

var isBackgroundReplacementActive: Bool

A Boolean value that indicates whether Background Replacement is currently active on a capture device.

class var isBackgroundReplacementEnabled: Bool

A class property that indicates whether a person enables the Background Replacement feature for this app.

