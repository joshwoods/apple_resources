

- AVFAudio
-  AVAudioApplication 

Class

# AVAudioApplication

An object that manages one or more audio sessions that belong to an app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class AVAudioApplication
```

## Overview

Access the shared audio application instance to control app-level audio operations, such as requesting microphone permission and controlling audio input muting.

## Topics

### Accessing the shared instance

class var shared: AVAudioApplication

Accesses the shared audio application instance.

### Requesting audio recording permission

class func requestRecordPermission(completionHandler: (Bool) -> Void)

Determines whether the app has permission to record audio.

var recordPermission: AVAudioApplication.recordPermission

The app’s permission to record audio.

enum recordPermission

Constants that indicate the app’s permission to record audio.

### Requesting microphone injection permission

class func requestMicrophoneInjectionPermission(completionHandler: (AVAudioApplication.MicrophoneInjectionPermission) -> Void)

Requests the app’s permission to add audio to calls.

var microphoneInjectionPermission: AVAudioApplication.MicrophoneInjectionPermission

A value that indicates an app’s permission to add audio to calls.

enum MicrophoneInjectionPermission

Constants that indicate an app’s permission to add audio to calls.

### Managing audio input mute state

var isInputMuted: Bool

A Boolean value that indicates whether the app’s audio input is in a muted state.

func setInputMuted(Bool) throws

Sets a Boolean value that indicates whether the app’s audio input is in a muted state.

class let inputMuteStateChangeNotification: NSNotification.Name

A notification the system posts when the app’s audio input mute state changes.

func setInputMuteStateChangeHandler(((Bool) -> Bool)?) throws

Sets a callback to handle changes to application-level audio muting states.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

class AVAudioSession

An object that communicates to the system how you intend to use audio in your app.

class AVAudioRoutingArbiter

An object for configuring macOS apps to participate in AirPods Automatic Switching.

