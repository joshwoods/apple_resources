

- AVFAudio
-  AVAudioSession 

Class

# AVAudioSession

An object that communicates to the system how you intend to use audio in your app.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioSession
```

## Mentioned in 

Handling audio interruptions

Responding to audio route changes

## Overview

An audio session acts as an intermediary between your app and the operating system — and, in turn, the underlying audio hardware. You use an audio session to communicate to the operating system the general nature of your app’s audio without detailing the specific behavior or required interactions with the audio hardware. You delegate the management of those details to the audio session, which ensures that the operating system can best manage the user’s audio experience.

All iOS, tvOS, and watchOS apps have a default audio session that comes preconfigured with the following behavior:

- It supports audio playback, but disallows audio recording.

- When the app plays audio, it silences any other background audio.

- In iOS, setting the Ring/Silent switch to silent mode silences any audio the app is playing.

- In iOS, locking a device silences the app’s audio.

Although the default audio session provides useful behavior, it generally doesn’t provide the audio behavior a media app needs. To change the default behavior, you configure your app’s audio session category.

There are six possible categories you can use, but playback is the one that playback apps most commonly use. This category indicates that audio playback is a central feature of your app. When you specify this category, your app’s audio continues with the Ring/Silent switch set to silent mode (iOS only). Using this category, you can also play background audio if you’re using the Audio, AirPlay, and Picture in Picture background mode. For more information, see `Enabling Background Audio`.

You use an AVAudioSession object to configure your app’s audio session. This class is a singleton object used to set the audio session’s category, mode, and other configurations. You can interact with the audio session throughout your app’s life cycle, but it’s often useful to perform this configuration at app launch, as shown in the following example.

```
func configureAudioSession() {
    // Retrieve the shared audio session.
    let audioSession = AVAudioSession.sharedInstance()
    do {
        // Set the audio session category and mode.
        try audioSession.setCategory(.playback, mode: .moviePlayback)
    } catch {
        print("Failed to set the audio session configuration")
    }
}
```

The audio session uses this configuration when you activate the session using the setActive:error: or setActive(_:options:) method.

Note

You can activate the audio session at any time after setting its category, but it’s generally preferable to defer this call until your app begins audio playback. Deferring the call ensures that you won’t prematurely interrupt any other background audio that may be in progress.

## Topics

### Accessing the shared audio session

class func sharedInstance() -> AVAudioSession

Returns the shared audio session instance.

### Configuring standard audio behaviors

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws

Sets the session category, mode, route-sharing policy, and options.

func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category, mode, and options.

func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws

Sets the audio session’s category with the specified options.

func setCategory(AVAudioSession.Category) throws

Sets the audio session’s category.

func setMode(AVAudioSession.Mode) throws

Sets the audio session’s mode.

### Configuring the spatial experience in visionOS

func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws

Sets the spatial audio experience your app intends to provide the user.

var intendedSpatialExperience: any AVAudioSessionSpatialExperience

The spatial audio experience your app intends to provide the user.

protocol AVAudioSessionSpatialExperience

A protocol that defines types of spatial audio experiences that the system supports.

struct HeadTrackedSpatialExperience

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

struct FixedSpatialExperience

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

struct BypassedSpatialExperience

An experience that bypasses system-provided audio spatialization.

enum AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

enum SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

var isNowPlayingCandidate: Bool

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

func setIsNowPlayingCandidate(Bool) throws

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

### Activating the audio configuration

func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws

Activates or deactivates your app’s audio session using the specified options.

func activate(options: AVAudioSessionActivationOptions, completionHandler: (Bool, (any Error)?) -> Void)

Activates an audio session asynchronously on watchOS.

struct AVAudioSessionActivationOptions

Constants that describe the options to pass when activating the audio session.

### Inspecting the category configuration

var category: AVAudioSession.Category

The current audio session category.

var availableCategories: [AVAudioSession.Category]

The audio session categories available on the current device.

struct Category

Audio session category identifiers.

var categoryOptions: AVAudioSession.CategoryOptions

The set of options associated with the current audio session category.

struct CategoryOptions

Constants that specify optional audio behaviors.

### Inspecting mode configuration

var mode: AVAudioSession.Mode

The current audio session’s mode.

var availableModes: [AVAudioSession.Mode]

The audio session modes available on the device.

struct Mode

Audio session mode identifiers.

### Inspecting rendering mode and capabilities

var renderingMode: AVAudioSession.RenderingMode

The current audio session’s rendering mode.

enum RenderingMode

Audio session rendering mode identifiers.

class let renderingModeChangeNotification: NSNotification.Name

A notification the system posts when the rendering mode changes.

var supportedOutputChannelLayouts: [AVAudioChannelLayout]

The array of channel layouts that the current route supports.

class let renderingCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when the rendering capabilities change.

### Inspecting the route sharing policy

var routeSharingPolicy: AVAudioSession.RouteSharingPolicy

The active route-sharing policy.

enum RouteSharingPolicy

Cases that indicate the possible route-sharing policies for an audio session.

### Mixing with other audio

var isOtherAudioPlaying: Bool

A Boolean value that indicates whether another app is playing audio.

var secondaryAudioShouldBeSilencedHint: Bool

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

var allowHapticsAndSystemSoundsDuringRecording: Bool

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

func setAllowHapticsAndSystemSoundsDuringRecording(Bool) throws

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

### Managing audio routing

Audio routing

Inspect and configure audio routes, ports, and data sources.

### Preparing for long-form video playback

func prepareRouteSelectionForPlayback(completionHandler: (Bool, AVAudioSession.RouteSelection) -> Void)

Prepares the route selection for long-form video playback.

enum RouteSelection

Constants used to define the active route selection.

### Handling interruptions

var prefersNoInterruptionsFromSystemAlerts: Bool

A Boolean value that indicates a preference for not interrupting the session with system alerts.

func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws

Sets the preference for not interrupting the audio session with system alerts.

var prefersInterruptionOnRouteDisconnect: Bool

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

func setPrefersInterruptionOnRouteDisconnect(Bool) throws

Sets a preference to interrupt the audio session when the active route disconnects.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

### Monitoring spatial capabilities

class let spatialPlaybackCapabilitiesChangedNotification: NSNotification.Name

A notification the system posts when its spatial playback capabilities change.

### Inspecting the audio prompt style

var promptStyle: AVAudioSession.PromptStyle

A hint to audio sessions that use voice prompt mode to alter the type of prompts they issue in response to other system audio, such as Siri and phone calls.

enum PromptStyle

Constants that indicate the prompt style to use.

### Enabling stereo recording

var inputOrientation: AVAudioSession.StereoOrientation

An orientation value that dictates which directions represent left and right when capturing audio from a built-in microphone configured for stereo recording.

var preferredInputOrientation: AVAudioSession.StereoOrientation

The audio session’s preferred stereo input orientation.

func setPreferredInputOrientation(AVAudioSession.StereoOrientation) throws

Sets the audio session’s preferred stereo input orientation.

enum StereoOrientation

Constants that define the supported stereo orientations.

### Enabling adding audio to calls

var isMicrophoneInjectionAvailable: Bool

A Boolean value that indicates whether microphone injection is available.

var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode

The preferred mode of injecting audio into another app’s input stream.

func setPreferredMicrophoneInjectionMode(AVAudioSession.MicrophoneInjectionMode) throws

Sets the preferred mode of injecting audio into another app’s input stream.

enum MicrophoneInjectionMode

The modes of injecting audio into another app’s input stream.

class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name

A notification the system posts when its capability to inject audio into an input stream changes.

### Configuring echo cancellation

var isEchoCancelledInputAvailable: Bool

A Boolean value that indicates whether the built-in microphone and speaker route supports echo cancellation.

var isEchoCancelledInputEnabled: Bool

A Boolean value that indicates whether an echo-canceled input is in an enabled state.

func setPrefersEchoCancelledInput(Bool) throws

Sets a preference to enable echo-canceled input on supported hardware.

var prefersEchoCancelledInput: Bool

A Boolean value that indicates the audio session’s preference for using an echo-canceled input.

### Configuring device settings

Audio hardware

Inspect and configure audio device settings including input gain, sample rate, and channel counts.

### Setting the aggregated I/O preference

func setAggregatedIOPreference(AVAudioSession.IOType) throws

Sets the audio session’s aggregated I/O configuration preference.

enum IOType

Constant values used to specify the audio session’s aggregated I/O behavior.

### Handling a change of media services

class let mediaServicesWereResetNotification: NSNotification.Name

A notification the system posts when the media server restarts.

class let mediaServicesWereLostNotification: NSNotification.Name

A notification the system posts when it terminates the media server.

### Errors

enum ErrorCode

Codes that describe error conditions that may occur when performing audio session operations.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

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

class AVAudioApplication

An object that manages one or more audio sessions that belong to an app.

class AVAudioRoutingArbiter

An object for configuring macOS apps to participate in AirPods Automatic Switching.

