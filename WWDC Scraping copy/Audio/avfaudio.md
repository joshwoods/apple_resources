<!--
Downloaded via https://llm.codes by @steipete on June 19, 2025 at 07:00 PM
Source URL: https://developer.apple.com/documentation/avfaudio
Total pages processed: 200
URLs filtered: Yes
Content de-duplicated: Yes
Availability strings filtered: Yes
Code blocks only: No
-->

# https://developer.apple.com/documentation/avfaudio

Framework

# AVFAudio

Play, record, and process audio; configure your app’s system audio behavior.

## Topics

### Essentials

AVFAudio updates

Learn about important changes to AVFAudio.

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

### Basic playback and recording

`class AVAudioPlayer`

An object that plays audio data from a file or buffer.

`class AVAudioRecorder`

An object that records audio data to a file.

`class AVMIDIPlayer`

An object that plays MIDI data through a system sound module.

### Advanced audio processing

Perform advanced real-time and offline audio processing, implement 3D spatialization, and work with MIDI and samplers.

### Speech synthesis

Configure voices to speak strings of text.

### Classes

`class AVAudioSessionCapability`

Describes whether a specific capability is supported and if that capability is currently enabled

Beta

`class AVAudioSessionPortExtensionBluetoothMicrophone`

An object that describes capabilities of Bluetooth microphone ports.

### Protocols

`protocol AVAudioSessionSpatialExperience`

### Variables

`var AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation: Int`

A flag that indicates that when your audio session deactivates, any audio sessions that your audio session interrupted can reactivate themselves.

Deprecated

`let AVEncoderASPFrequencyKey: String` Beta

`let AVEncoderContentSourceKey: String` Beta

`let AVEncoderDynamicRangeControlConfigurationKey: String` Beta

`let AVSampleRateConverterAlgorithm_Mastering: String`

The mastering encoder bit rate strategy.

`let AVSampleRateConverterAlgorithm_MinimumPhase: String`

The minimum phase encoder bit rate strategy.

`let AVSampleRateConverterAlgorithm_Normal: String`

The usual encoder bit rate strategy.

### Functions

Creates a beat range with the specified start time and length.

### Type Aliases

`typealias AVAudioConverterInputBlock`

A block to get input data for conversion, as necessary.

`typealias AVBeatRange`

`typealias AVMIDIPlayerCompletionHandler`

A callback the system invokes when MIDI playback completes.

### Enumerations

`enum AVAudioContentSource` Beta

`enum AVAudioDynamicRangeControlConfiguration`

---

# https://developer.apple.com/documentation/avfaudio/handling-audio-interruptions

- AVFAudio
- Handling audio interruptions

Article

# Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

## Overview

Interruptions are a common part of the iOS and watchOS user experiences. For example, consider the scenario of receiving a phone call while you’re watching a movie in the TV app on your iPhone. In this case, the movie’s audio fades out, playback pauses, and the sound of the call’s ringtone fades in. If you decline the call, control returns to the TV app, and playback begins again as the movie’s audio fades in.

At the center of this behavior is your app’s audio session. As interruptions begin and end, the audio session notifies any registered observers so they can take appropriate action. For example, `AVPlayer` monitors your app’s audio session and automatically pauses playback in response to interruption events. You can monitor these changes by key-value observing the player’s `timeControlStatus` property, and update your user interface as necessary when the player pauses and resumes playback.

### Customize the interruption behavior

Most apps rely on the system’s default interruption behavior. However, `AVAudioSession` provides ways to customize the default behavior to better accommodate your app’s needs:

- Recent iPad models provide a feature that mutes the built-in microphone at the hardware level when the user closes the device’s Smart Folio cover. If your app plays and records audio, you may want to continue playback even if the system mutes the microphone. You can disable the default interruption behavior by setting the `overrideMutedMicrophoneInterruption` option when configuring your audio session.

- System alerts, such as receiving an incoming phone call, interrupt the active audio session. If you prefer that the system not interrupt your app’s audio session in these cases, you can indicate this preference by setting a value for the `setPrefersNoInterruptionsFromSystemAlerts(_:)` method.

### Observe audio session interruptions

You can directly observe interruption notifications that `AVAudioSession` posts. This might be useful if you want to know when the system pauses playback due to an interruption or another reason, such as a route change. To observe audio interruptions, begin by registering to observe notifications of type `interruptionNotification`.

func setupNotifications() {
// Get the default notification center instance.
let nc = NotificationCenter.default
nc.addObserver(self,
selector: #selector(handleInterruption),
name: AVAudioSession.interruptionNotification,
object: AVAudioSession.sharedInstance())
}

@objc func handleInterruption(notification: Notification) {
// To implement.
}

### Handle audio session interruptions

The posted `Notification` object contains a populated user-information dictionary that provides the details of the interruption. You determine the type of interruption by retrieving the `AVAudioSession.InterruptionType` value from the `userInfo` dictionary. The interruption type indicates whether the interruption is beginning or ending.

@objc func handleInterruption(notification: Notification) {
guard let userInfo = notification.userInfo,
let typeValue = userInfo[AVAudioSessionInterruptionTypeKey] as? UInt,
let type = AVAudioSession.InterruptionType(rawValue: typeValue) else {
return
}

// Switch over the interruption type.
switch type {

case .began:
// An interruption began. Update the UI as necessary.

case .ended:
// An interruption ended. Resume playback, if appropriate.

guard let optionsValue = userInfo[AVAudioSessionInterruptionOptionKey] as? UInt else { return }
let options = AVAudioSession.InterruptionOptions(rawValue: optionsValue)
if options.contains(.shouldResume) {
// An interruption ended. Resume playback.
} else {
// An interruption ended. Don't resume playback.
}

default: ()
}
}

If the interruption type is `AVAudioSession.InterruptionType.ended`, the `userInfo` dictionary contains an `AVAudioSession.InterruptionOptions` value, which you use to determine whether playback automatically resumes.

## See Also

### System audio

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

---

# https://developer.apple.com/documentation/avfaudio/responding-to-audio-route-changes

- AVFAudio
- Responding to audio route changes

Article

# Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

## Overview

An important responsibility of `AVAudioSession` is managing audio route changes. A route change occurs when the system adds or removes an audio input or output. Route changes occur for several reasons, including a user plugging in a pair of headphones, connecting a Bluetooth LE headset, or unplugging a USB audio interface. When these changes occur, the audio session reroutes audio signals accordingly and broadcasts a notification containing the details of the change to any registered observers.

An important behavior related to route changes occurs when a user plugs in or removes a pair of headphones (see Playing audio in Human Interface Guidelines). When users connect a pair of wired or wireless headphones, they’re implicitly indicating that audio playback should continue, but privately. They expect an app that’s currently playing media to continue playing without pause. However, when users _disconnect_ their headphones, they don’t want to automatically share what they’re listening to with others. Applications should respect this implicit privacy request and automatically pause playback when users disconnect their headphones.

### Observe route changes

You can directly observe route change notifications posted by the audio session. This might be useful if you want the system to notify you when a user connects headphones so you can present an icon or message in the player interface.

To observe audio route changes, begin by registering to observe notifications of type `routeChangeNotification`.

func setupNotifications() {
// Get the default notification center instance.
let nc = NotificationCenter.default
nc.addObserver(self,
selector: #selector(handleRouteChange),
name: AVAudioSession.routeChangeNotification,
object: nil)
}

@objc func handleRouteChange(notification: Notification) {
// To be implemented.
}

### Respond to route changes

The posted `Notification` object contains a populated user-information dictionary providing the details of the route change. Determine the reason for this change by retrieving the `AVAudioSession.RouteChangeReason` value from the dictionary. When a user connects a new device, the reason is `AVAudioSession.RouteChangeReason.newDeviceAvailable`, and when a user removes a device, the reason is `AVAudioSession.RouteChangeReason.oldDeviceUnavailable`.

When a new device becomes available, you ask the audio session for its `currentRoute` to determine where the audio output is currently routed. This query returns an `AVAudioSessionRouteDescription` object that lists all of the audio session’s inputs and outputs. When the user removes a device, you retrieve the route description for the previous route from the user-information dictionary. In both cases, you query the route description for its outputs, which returns an array of port description objects providing the details of the audio output routes.

@objc func handleRouteChange(notification: Notification) {
guard let userInfo = notification.userInfo,
let reasonValue = userInfo[AVAudioSessionRouteChangeReasonKey] as? UInt,
let reason = AVAudioSession.RouteChangeReason(rawValue: reasonValue) else {
return
}

// Switch over the route change reason.
switch reason {

case .newDeviceAvailable: // New device found.
let session = AVAudioSession.sharedInstance()
headphonesConnected = hasHeadphones(in: session.currentRoute)

case .oldDeviceUnavailable: // Old device removed.
if let previousRoute =
userInfo[AVAudioSessionRouteChangePreviousRouteKey] as? AVAudioSessionRouteDescription {
headphonesConnected = hasHeadphones(in: previousRoute)
}

default: ()
}
}

// Filter the outputs to only those with a port type of headphones.
return !routeDescription.outputs.filter({$0.portType == .headphones}).isEmpty
}

## See Also

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

---

# https://developer.apple.com/documentation/avfaudio/adding-synthesized-speech-to-calls

- AVFAudio
- Adding synthesized speech to calls

Sample Code

# Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Download

Xcode 16.1+

## Overview

This sample shows how to create an accessibility app that supports augmentative and alternative communication (AAC) by adding synthesized speech to a call. This feature is available in iOS 18.2 and visionOS 2.2 and later, and is available to use with calling apps that capture microphone input using Apple’s voice processing like Phone, FaceTime, and most VoIP apps.

The sample app provides a basic user interface with a button to toggle the feature state and a text field. When you enter text into the field and press enter, the app speaks the phrase. If you have an active call in progress and you enable adding the app’s audio to it, you’ll hear the synthesized speech on the originating and receiving ends of the call.

## Configure the sample code project

The sample requires running on an iOS device with iOS 18.2 or later. To test the sample, establish a phone or FaceTime call with another device.

## Enable the accessibility service

The sample determines the state of this setting by querying the shared `AVAudioApplication` object for its microphone injection permission:

// Retrieve the current microphone injection permission.
let permission = AVAudioApplication.shared.microphoneInjectionPermission

A permission value of `AVAudioApplication.MicrophoneInjectionPermission.serviceDisabled` indicates the person hasn’t turned on the service, which means apps can’t add audio to calls. When the app retrieves this value, it presents an alert dialog that indicates the current state and provides the person an opportunity to update their setting. When you press the dialog’s Open Settings button, the app uses the Accessibility framework to directly open the Add Audio in Calls screen in the Settings app like shown below.

@ViewBuilder
var alertButtons: some View {
Button("Open Settings") {
Task {
do {
// Open the configuration screen for this feature in the Settings app.
try await AccessibilitySettings.openSettings(for: .allowAppsToAddAudioToCalls)
} catch {
print("Unable to open Settings app: \(error)")
}
}
}
Button("Cancel", role: .cancel) {}
}

## Request permission

Turning on Add Audio in Calls makes the feature available to apps on the system, but apps must explicitly request and be granted permission to use the feature. The sample determines its permission by querying for the current microphone injection permission. A value of `AVAudioApplication.MicrophoneInjectionPermission.undetermined` indicates the app hasn’t yet requested permission and needs to before it can use the feature.

For an app to request a person’s permission, it needs to provide an `NSMicrophoneInjectionUsageDescription` key in its `Info.plist` file with a description of why the app requests microphone access. The system displays this string when an app requests user permission. The sample app defines this entry as follows.

Attempting to request permission without this usage string present results in the system quitting the app.

The app requests permission by calling the `requestRecordPermission(completionHandler:)` method and awaiting a response:

// If undetermined, prompt the person to grant the app access, and turn on the feature, if allowed.
if await AVAudioApplication.requestMicrophoneInjectionPermission() == .granted {
// If the person grants access, turn on adding app audio.
}

Calling this method causes the system to present a dialog that requests user permission. If a person grants the app permission, the call returns a value of `AVAudioApplication.MicrophoneInjectionPermission.granted` and the app updates its state accordingly.

If a person denies the app permission, the system sets the microphone injection permission state to `AVAudioApplication.MicrophoneInjectionPermission.denied`, and the app is unable to use the feature. The app remains in this state until a person explicitly changes the permission from the Add Audio in Calls screen in the Settings app. If you attempt to turn on the feature in the app while in this state, the app presents an alert similar to the one shown in the previous section to update the app’s permission.

## Enable adding audio to calls

When the app has permission to add audio and a person toggles the feature state in the user interface, the app responds by calling the shared `AVAudioSession` object’s `setPreferredMicrophoneInjectionMode(_:)` method. To turn on the feature, the app passes the method a value of `AVAudioSession.MicrophoneInjectionMode.spokenAudio`; to turn off the feature, it passes a value of `AVAudioSession.MicrophoneInjectionMode.none`.

let mode: AVAudioSession.MicrophoneInjectionMode = // spoken audio or none
try AVAudioSession.sharedInstance().setPreferredMicrophoneInjectionMode(mode)

When turned on during an active call, the system plays the app’s audio locally and adds it to the microphone’s input stream.

## Monitor the availability of calls

To determine whether a call can use this feature, the sample awaits notification of changes to the state of the audio session’s microphone injection capabilities:

/// Monitor the active state of phone and FaceTime calls.
private func observeCallState() async {
// Await notification of changes to the audio session's microphone injection capabilities.
for await notification in NotificationCenter.default.notifications(named: AVAudioSession.microphoneInjectionCapabilitiesChangeNotification) {
// Inspect the user information dictionary to determine whether microphone injection is available.
isCallActive = notification.userInfo?[AVAudioSessionMicrophoneInjectionIsAvailableKey] as? Bool ?? false
}
}

When a call begins or ends, the system posts a notification of the change. The app queries the notification’s user information dictionary for its `AVAudioSessionMicrophoneInjectionIsAvailableKey` value to determine whether there’s an active call. When the value is `true`, the app updates its UI to show a pulsing phone icon in the toolbar to indicate the call is active.

## See Also

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

---

# https://developer.apple.com/documentation/avfaudio/capturing-stereo-audio-from-built-in-microphones

- AVFAudio
- Capturing stereo audio from built-In microphones

Sample Code

# Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

Download

Xcode 15.4+

## Overview

Stereo audio uses two channels to create the illusion of multidirectional sound, adding greater depth and dimension to your audio and resulting in an immersive listening experience. iOS provides a number of ways to record audio from the built-in microphones, but until now it’s been limited to mono audio only. Starting in iOS 14 and iPadOS 14, you can now capture stereo audio using the built-in microphones on supported devices.

Because a user can hold an iOS device in a variety of ways, you need to specify the orientation of the right and left channels in the stereo field. Set the built-in microphone’s directionality by configuring:

- Polar pattern. The system represents the individual device microphones, and beamformers that use multiple microphones, as data sources. Select the front or back data source and set its polar pattern to stereo.

- Input orientation. When recording video, set the input orientation to match the video orientation. When recording audio only, set the input orientation to match the user interface orientation. In both cases, don’t change the orientation during recording.

This sample app shows how to configure your app to record stereo audio, and helps you visualize changes to the input orientation and data-source selection.

### Configure the Audio Session Category

Recording stereo audio requires the app’s audio session to use either the record or playAndRecord category. The sample uses the `playAndRecord` category so it can do both. It also passes the `defaultToSpeaker` and `allowBluetooth` options to route the audio to the speaker instead of the receiver, and to Bluetooth headphones.

func setupAudioSession() {
do {
let session = AVAudioSession.sharedInstance()
try session.setCategory(.playAndRecord, options: [.defaultToSpeaker, .allowBluetooth])
try session.setActive(true)
} catch {
fatalError("Failed to configure and activate session.")
}
}

### Select and Configure a Built-In Microphone

An iOS device’s built-in microphone input consists of an array of physical microphones and beamformers, each represented as an instance of `AVAudioSessionDataSourceDescription`. The sample app finds the built-in microphone input by querying the available inputs for the one where the port type equals the built-in microphone, and sets it as the preferred input.

private func enableBuiltInMic() {
// Get the shared audio session.
let session = AVAudioSession.sharedInstance()

// Find the built-in microphone input.
guard let availableInputs = session.availableInputs,
let builtInMicInput = availableInputs.first(where: { $0.portType == .builtInMic }) else {
print("The device must have a built-in microphone.")
return
}

// Make the built-in microphone input the preferred input.
do {
try session.setPreferredInput(builtInMicInput)
} catch {
print("Unable to set the built-in mic as the preferred input.")
}
}

### Configure the Microphone Input’s Directionality

To configure the microphone input’s directionality, the sample sets its data source’s preferred polar pattern and the session’s input orientation. It performs this configuration in its `selectRecordingOption(_:orientation)` method, which it calls whenever the user rotates the device or changes the recording option selection.

// Get the shared audio session.
let session = AVAudioSession.sharedInstance()

// Find the built-in microphone input's data sources,
// and select the one that matches the specified name.
guard let preferredInput = session.preferredInput,
let dataSources = preferredInput.dataSources,
let newDataSource = dataSources.first(where: { $0.dataSourceName == option.dataSourceName }),
let supportedPolarPatterns = newDataSource.supportedPolarPatterns else {
completion(.none)
return
}

do {
isStereoSupported = supportedPolarPatterns.contains(.stereo)
// If the data source supports stereo, set it as the preferred polar pattern.
if isStereoSupported {
// Set the preferred polar pattern to stereo.
try newDataSource.setPreferredPolarPattern(.stereo)
}

// Set the preferred data source and polar pattern.
try preferredInput.setPreferredDataSource(newDataSource)

// Update the input orientation to match the current user interface orientation.
try session.setPreferredInputOrientation(orientation.inputOrientation)

} catch {
fatalError("Unable to select the \(option.dataSourceName) data source.")
}

// Call the completion handler with the updated stereo layout.
completion(StereoLayout(orientation: newDataSource.orientation!,
stereoOrientation: session.inputOrientation))
}

This method finds the data source with the selected name, sets its preferred polar pattern to stereo, and then sets it as the input’s preferred data source. Finally, it sets the preferred input orientation to match the device’s user interface orientation.

## See Also

### System audio

Handling audio interruptions

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Responding to audio route changes

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession

- AVFAudio
- AVAudioSession

Class

# AVAudioSession

An object that communicates to the system how you intend to use audio in your app.

class AVAudioSession

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

There are six possible categories you can use, but `playback` is the one that playback apps most commonly use. This category indicates that audio playback is a central feature of your app. When you specify this category, your app’s audio continues with the Ring/Silent switch set to silent mode (iOS only). Using this category, you can also play background audio if you’re using the Audio, AirPlay, and Picture in Picture background mode. For more information, see `Enabling Background Audio`.

You use an `AVAudioSession` object to configure your app’s audio session. This class is a singleton object used to set the audio session’s category, mode, and other configurations. You can interact with the audio session throughout your app’s life cycle, but it’s often useful to perform this configuration at app launch, as shown in the following example.

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

The audio session uses this configuration when you activate the session using the `setActive:error:` or `setActive(_:options:)` method.

## Topics

### Accessing the shared audio session

Returns the shared audio session instance.

### Configuring standard audio behaviors

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws`

Sets the session category, mode, route-sharing policy, and options.

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category, mode, and options.

`func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category with the specified options.

`func setCategory(AVAudioSession.Category) throws`

Sets the audio session’s category.

`func setMode(AVAudioSession.Mode) throws`

Sets the audio session’s mode.

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

### Activating the audio configuration

`func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws`

Activates or deactivates your app’s audio session using the specified options.

Activates an audio session asynchronously on watchOS.

`struct AVAudioSessionActivationOptions`

Constants that describe the options to pass when activating the audio session.

### Inspecting the category configuration

`var category: AVAudioSession.Category`

The current audio session category.

[`var availableCategories: [AVAudioSession.Category]`](https://developer.apple.com/documentation/avfaudio/avaudiosession/availablecategories)

The audio session categories available on the current device.

`struct Category`

Audio session category identifiers.

`var categoryOptions: AVAudioSession.CategoryOptions`

The set of options associated with the current audio session category.

`struct CategoryOptions`

Constants that specify optional audio behaviors.

### Inspecting mode configuration

`var mode: AVAudioSession.Mode`

The current audio session’s mode.

[`var availableModes: [AVAudioSession.Mode]`](https://developer.apple.com/documentation/avfaudio/avaudiosession/availablemodes)

The audio session modes available on the device.

`struct Mode`

Audio session mode identifiers.

### Inspecting rendering mode and capabilities

`var renderingMode: AVAudioSession.RenderingMode`

The current audio session’s rendering mode.

`enum RenderingMode`

Audio session rendering mode identifiers.

`class let renderingModeChangeNotification: NSNotification.Name`

A notification the system posts when the rendering mode changes.

[`var supportedOutputChannelLayouts: [AVAudioChannelLayout]`](https://developer.apple.com/documentation/avfaudio/avaudiosession/supportedoutputchannellayouts)

The array of channel layouts that the current route supports.

`class let renderingCapabilitiesChangeNotification: NSNotification.Name`

A notification the system posts when the rendering capabilities change.

### Inspecting the route sharing policy

`var routeSharingPolicy: AVAudioSession.RouteSharingPolicy`

The active route-sharing policy.

`enum RouteSharingPolicy`

Cases that indicate the possible route-sharing policies for an audio session.

### Mixing with other audio

`var isOtherAudioPlaying: Bool`

A Boolean value that indicates whether another app is playing audio.

`var secondaryAudioShouldBeSilencedHint: Bool`

A Boolean value that indicates whether another app, with a nonmixable audio session, is playing audio.

`class let silenceSecondaryAudioHintNotification: NSNotification.Name`

A notification the system posts when the primary audio from other apps starts and stops.

`var allowHapticsAndSystemSoundsDuringRecording: Bool`

A Boolean value that indicates whether system sounds and haptics play while recording from audio input.

`func setAllowHapticsAndSystemSoundsDuringRecording(Bool) throws`

Sets a Boolean value that indicates whether system sounds and haptics play while recording from audio input.

### Managing audio routing

Inspect and configure audio routes, ports, and data sources.

### Preparing for long-form video playback

Prepares the route selection for long-form video playback.

`enum RouteSelection`

Constants used to define the active route selection.

### Handling interruptions

`var prefersNoInterruptionsFromSystemAlerts: Bool`

A Boolean value that indicates a preference for not interrupting the session with system alerts.

`func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws`

Sets the preference for not interrupting the audio session with system alerts.

`var prefersInterruptionOnRouteDisconnect: Bool`

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

`func setPrefersInterruptionOnRouteDisconnect(Bool) throws`

Sets a preference to interrupt the audio session when the active route disconnects.

`class let interruptionNotification: NSNotification.Name`

A notification the system posts when an audio interruption occurs.

### Monitoring spatial capabilities

`class let spatialPlaybackCapabilitiesChangedNotification: NSNotification.Name`

A notification the system posts when its spatial playback capabilities change.

### Inspecting the audio prompt style

`var promptStyle: AVAudioSession.PromptStyle`

A hint to audio sessions that use voice prompt mode to alter the type of prompts they issue in response to other system audio, such as Siri and phone calls.

`enum PromptStyle`

Constants that indicate the prompt style to use.

### Enabling stereo recording

`var inputOrientation: AVAudioSession.StereoOrientation`

An orientation value that dictates which directions represent left and right when capturing audio from a built-in microphone configured for stereo recording.

`var preferredInputOrientation: AVAudioSession.StereoOrientation`

The audio session’s preferred stereo input orientation.

`func setPreferredInputOrientation(AVAudioSession.StereoOrientation) throws`

Sets the audio session’s preferred stereo input orientation.

`enum StereoOrientation`

Constants that define the supported stereo orientations.

### Enabling adding audio to calls

`var isMicrophoneInjectionAvailable: Bool`

A Boolean value that indicates whether microphone injection is available.

`var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode`

The preferred mode of injecting audio into another app’s input stream.

`func setPreferredMicrophoneInjectionMode(AVAudioSession.MicrophoneInjectionMode) throws`

Sets the preferred mode of injecting audio into another app’s input stream.

`enum MicrophoneInjectionMode`

The modes of injecting audio into another app’s input stream.

`class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name`

A notification the system posts when its capability to inject audio into an input stream changes.

### Configuring echo cancellation

`var isEchoCancelledInputAvailable: Bool`

A Boolean value that indicates whether the built-in microphone and speaker route supports echo cancellation.

`var isEchoCancelledInputEnabled: Bool`

A Boolean value that indicates whether an echo-canceled input is in an enabled state.

`func setPrefersEchoCancelledInput(Bool) throws`

Sets a preference to enable echo-canceled input on supported hardware.

`var prefersEchoCancelledInput: Bool`

A Boolean value that indicates the audio session’s preference for using an echo-canceled input.

### Configuring device settings

Inspect and configure audio device settings including input gain, sample rate, and channel counts.

### Setting the aggregated I/O preference

`func setAggregatedIOPreference(AVAudioSession.IOType) throws`

Sets the audio session’s aggregated I/O configuration preference.

`enum IOType`

Constant values used to specify the audio session’s aggregated I/O behavior.

### Handling a change of media services

`class let mediaServicesWereResetNotification: NSNotification.Name`

A notification the system posts when the media server restarts.

`class let mediaServicesWereLostNotification: NSNotification.Name`

A notification the system posts when it terminates the media server.

### Errors

`enum ErrorCode`

Codes that describe error conditions that may occur when performing audio session operations.

### Deprecated

Review unsupported symbols and their replacements.

### Instance Properties

`var intendedSpatialExperience: any AVAudioSessionSpatialExperience`

the developer’s intended spatial experience for this audio session

`var isOutputMuted: Bool`

A Boolean value that indicates whether audio output is in a muted state.

Beta

### Instance Methods

`func setOutputMuted(Bool) throws`

Sets a Boolean value to inform the system to mute the session’s output audio. The default value is false (unmuted).

### Type Properties

`class let availableInputsChangeNotification: NSNotification.Name` Beta

`class let muteStateKey: String`

Keys for `outputMuteStateChangeNotification` Value is `NSNumber` type with boolean value 0 for unmuted or value 1 for muted (samples zeroed out)

`class let outputMuteStateChangeNotification: NSNotification.Name`

Notification sent to registered listeners when session’s output mute state changes.

`class let userIntentToUnmuteOutputNotification: NSNotification.Name`

Notification sent to registered listeners when the application’s output is muted and user hints to unmute.

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`
- `Sendable`
- `SendableMetatype`

## See Also

### System audio

Observe audio session notifications to ensure that your app responds appropriately to interruptions.

Observe audio session notifications to ensure that your app responds appropriately to route changes.

Adding synthesized speech to calls

Provide a more accessible experience by adding your app’s audio to a call.

Capturing stereo audio from built-In microphones

Configure an iOS device’s built-in microphones to add stereo recording capabilities to your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication

- AVFAudio
- AVAudioApplication

Class

# AVAudioApplication

An object that manages one or more audio sessions that belong to an app.

class AVAudioApplication

## Overview

Access the shared audio application instance to control app-level audio operations, such as requesting microphone permission and controlling audio input muting.

## Topics

### Accessing the shared instance

`class var shared: AVAudioApplication`

Accesses the shared audio application instance.

### Requesting audio recording permission

Determines whether the app has permission to record audio.

`var recordPermission: AVAudioApplication.recordPermission`

The app’s permission to record audio.

`enum recordPermission`

Constants that indicate the app’s permission to record audio.

### Requesting microphone injection permission

Requests the app’s permission to add audio to calls.

`var microphoneInjectionPermission: AVAudioApplication.MicrophoneInjectionPermission`

A value that indicates an app’s permission to add audio to calls.

`enum MicrophoneInjectionPermission`

Constants that indicate an app’s permission to add audio to calls.

### Managing audio input mute state

`var isInputMuted: Bool`

A Boolean value that indicates whether the app’s audio input is in a muted state.

`func setInputMuted(Bool) throws`

Sets a Boolean value that indicates whether the app’s audio input is in a muted state.

`class let inputMuteStateChangeNotification: NSNotification.Name`

A notification the system posts when the app’s audio input mute state changes.

Sets a call

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`
- `Sendable`
- `SendableMetatype`

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

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioRoutingArbiter`

An object for configuring macOS apps to participate in AirPods Automatic Switching.

---

# https://developer.apple.com/documentation/avfaudio/avaudioroutingarbiter

- AVFAudio
- AVAudioRoutingArbiter

Class

# AVAudioRoutingArbiter

An object for configuring macOS apps to participate in AirPods Automatic Switching.

class AVAudioRoutingArbiter

## Overview

AirPods Automatic Switching is a feature of Apple operating systems that intelligently connects wireless headphones to the most appropriate audio device in a multidevice environment. For example, if a user plays a movie on iPad, and then locks the device and starts playing music on iPhone, the system automatically switches the source audio device from iPad to iPhone.

iOS apps automatically participate in AirPods Automatic Switching. To enable your macOS app to participate in this behavior, use `AVAudioRoutingArbiter` to indicate when your app starts and finishes playing or recording audio. For example, a Voice over IP (VoIP) app might request arbitration before starting a call, and when the arbitration completes, begin the VoIP session. Likewise, when the call ends, the app would end the VoIP session and leave arbitration.

func startCall() {
let arbiter = AVAudioRoutingArbiter.shared
arbiter.begin(category: .playAndRecordVoice) { deviceChanged, error in
// Start VoIP session.
}
}

func endCall() {
// End VoIP session.
AVAudioRoutingArbiter.shared.leave()
}

## Topics

### Creating a Routing Arbiter

`class var shared: AVAudioRoutingArbiter`

The shared routing arbiter object.

### Participating in AirPods Automatic Switching

Begins routing arbitration to take ownership of a nearby Bluetooth audio route.

`enum Category`

Categories that describe the general nature of your app’s audio use.

`func leave()`

Stops an app’s participation in audio routing arbitration.

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`
- `Sendable`
- `SendableMetatype`

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

`class AVAudioSession`

An object that communicates to the system how you intend to use audio in your app.

`class AVAudioApplication`

An object that manages one or more audio sessions that belong to an app.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer

- AVFAudio
- AVAudioPlayer

Class

# AVAudioPlayer

An object that plays audio data from a file or buffer.

class AVAudioPlayer

## Overview

Use an audio player to:

- Play audio of any duration from a file or buffer

- Control the volume, panning, rate, and looping behavior of the played audio

- Access playback-level metering data

- Play multiple sounds simultaneously by synchronizing the playback of multiple players

For more information about preparing your app to play audio, see Configuring your app for media playback.

## Topics

### Creating an audio player

`init(contentsOf: URL) throws`

Creates a player to play audio from a file.

`init(contentsOf: URL, fileTypeHint: String?) throws`

Creates a player to play audio from a file of a particular type.

`init(data: Data) throws`

Creates a player to play in-memory audio data.

`init(data: Data, fileTypeHint: String?) throws`

Creates a player to play in-memory audio data of a particular type.

### Controlling playback

Prepares the player for audio playback.

Plays audio asynchronously.

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

`func pause()`

Pauses audio playback.

`func stop()`

Stops playback and undoes the setup the system requires for playback.

`var isPlaying: Bool`

A Boolean value that indicates whether the player is currently playing audio.

### Configuring playback settings

`var volume: Float`

The audio player’s volume relative to other audio output.

`func setVolume(Float, fadeDuration: TimeInterval)`

Changes the audio player’s volume over a duration of time.

`var pan: Float`

The audio player’s stereo pan position.

`var enableRate: Bool`

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

`var rate: Float`

The audio player’s playback rate.

`var numberOfLoops: Int`

The number of times the audio repeats playback.

### Accessing player timing

`var currentTime: TimeInterval`

The current playback time, in seconds, within the audio timeline.

`var duration: TimeInterval`

The total duration, in seconds, of the player’s audio.

### Managing audio channels

`var numberOfChannels: Int`

The number of audio channels in the player’s audio.

[`var channelAssignments: [AVAudioSessionChannelDescription]?`](https://developer.apple.com/documentation/avfaudio/avaudioplayer/channelassignments)

An array of channel descriptions for the audio player.

### Managing audio-level metering

`var isMeteringEnabled: Bool`

A Boolean value that indicates whether the player is able to generate audio-level metering data.

`func updateMeters()`

Refreshes the average and peak power values for all channels of an audio player.

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

### Responding to player events

`var delegate: (any AVAudioPlayerDelegate)?`

The delegate object for the audio player.

`protocol AVAudioPlayerDelegate`

A protocol that defines the methods to respond to audio playback events and decoding errors.

### Inspecting the audio data

`var url: URL?`

The URL of the audio file.

`var data: Data?`

The audio data associated with the player.

`var format: AVAudioFormat`

The format of the player’s audio data.

[`var settings: [String : Any]`](https://developer.apple.com/documentation/avfaudio/avaudioplayer/settings)

A dictionary that provides information about the player’s audio data.

### Accessing device information

`var currentDevice: String?`

The unique identifier of the current audio player.

`var deviceCurrentTime: TimeInterval`

The time value, in seconds, of the audio output device’s clock.

### Instance Properties

`var intendedSpatialExperience: any SpatialAudioExperience`

The AVAudioPlayer’s intended spatial experience.

Beta

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`

## See Also

### Basic playback and recording

`class AVAudioRecorder`

An object that records audio data to a file.

`class AVMIDIPlayer`

An object that plays MIDI data through a system sound module.

---

# https://developer.apple.com/documentation/avfaudio/avaudiorecorder

- AVFAudio
- AVAudioRecorder

Class

# AVAudioRecorder

An object that records audio data to a file.

class AVAudioRecorder

## Overview

Use an audio recorder to:

- Record audio from the system’s active input device

- Record for a specified duration or until the user stops recording

- Pause and resume a recording

- Access recording-level metering data

To record audio in iOS or tvOS, configure your audio session to use the `record` or `playAndRecord` category.

## Topics

### Creating an audio recorder

[`init(url: URL, settings: [String : Any]) throws`](https://developer.apple.com/documentation/avfaudio/avaudiorecorder/init(url:settings:))

Creates an audio recorder with settings.

`init(url: URL, format: AVAudioFormat) throws`

Creates an audio recorder with an audio format.

### Controlling recording

Creates an audio file and prepares the system for recording.

Starts or resumes audio recording.

Records audio starting at a specific time.

Records audio for the indicated duration of time.

Records audio starting at a specific time for the indicated duration.

`func pause()`

Pauses an audio recording.

`func stop()`

Stops recording and closes the audio file.

`var isRecording: Bool`

A Boolean value that indicates whether the audio recorder is recording.

Deletes a recorded audio file.

### Accessing recorder timing

`var currentTime: TimeInterval`

The time, in seconds, since the beginning of the recording.

`var deviceCurrentTime: TimeInterval`

The time, in seconds, of the host audio device.

### Managing audio channels

[`var channelAssignments: [AVAudioSessionChannelDescription]?`](https://developer.apple.com/documentation/avfaudio/avaudiorecorder/channelassignments)

An array of channel descriptions associated with the audio recorder.

### Managing audio-level metering

`var isMeteringEnabled: Bool`

A Boolean value that indicates whether you’ve enabled the recorder to generate audio-level metering data.

`func updateMeters()`

Refreshes the average and peak power values for all channels of an audio recorder.

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

### Responding to recorder events

`var delegate: (any AVAudioRecorderDelegate)?`

The delegate object for the audio recorder.

`protocol AVAudioRecorderDelegate`

A protocol that defines the methods to respond to audio recording events and encoding errors.

### Inspecting the audio data

`var url: URL`

The URL to which the recorder writes its data.

`var format: AVAudioFormat`

The format of the recorded audio.

[`var settings: [String : Any]`](https://developer.apple.com/documentation/avfaudio/avaudiorecorder/settings)

The settings that describe the format of the recorded audio.

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`
- `Sendable`
- `SendableMetatype`

## See Also

### Basic playback and recording

`class AVAudioPlayer`

An object that plays audio data from a file or buffer.

`class AVMIDIPlayer`

An object that plays MIDI data through a system sound module.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer

- AVFAudio
- AVMIDIPlayer

Class

# AVMIDIPlayer

An object that plays MIDI data through a system sound module.

class AVMIDIPlayer

## Overview

For more information about preparing your app to play audio, see Configuring your app for media playback.

## Topics

### Creating a MIDI player

`init(contentsOf: URL, soundBankURL: URL?) throws`

Creates a player to play a MIDI file with the specified soundbank.

`init(data: Data, soundBankURL: URL?) throws`

Creates a player to play MIDI data with the specified soundbank.

### Controlling playback

`func prepareToPlay()`

Prepares the player to play the sequence by prerolling all events.

Plays the MIDI sequence.

`func stop()`

Stops playing the sequence.

`var isPlaying: Bool`

A Boolean value that indicates whether the sequence is playing.

### Configuring playback settings

`var rate: Float`

The playback rate of the player.

### Accessing player timing

`var currentPosition: TimeInterval`

The current playback position, in seconds.

`var duration: TimeInterval`

The duration, in seconds, of the currently loaded file.

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`

## See Also

### Basic playback and recording

`class AVAudioPlayer`

An object that plays audio data from a file or buffer.

`class AVAudioRecorder`

An object that records audio data to a file.

---

# https://developer.apple.com/documentation/avfaudio/audio-engine

Collection

- AVFAudio
- Audio Engine

API Collection

# Audio Engine

Perform advanced real-time and offline audio processing, implement 3D spatialization, and work with MIDI and samplers.

## Overview

The audio engine provides a powerful, feature-rich API to simplify audio generation, processing, and input/output tasks. The engine contains a group of nodes that connect to form an audio signal processing chain. These nodes perform a variety of tasks on a signal before rendering to an output destination.

Audio Engine helps you achieve simple, as well as complex, audio processing tasks. With Audio Engine, your apps can:

- Play audio using files and buffers

- Capture audio at any point during the processing chain

- Add built-in effects like reverb, delay, distortion, and your custom effects

- Perform stereo and 3D mixing

- Provide MIDI playback and control over sampler instruments

## Topics

### Essentials

`class AVAudioEngine`

An object that manages a graph of audio nodes, controls playback, and configures real-time rendering constraints.

### Nodes

`class AVAudioNode`

An object you use for audio generation, processing, or an I/O block.

`class AVAudioInputNode`

An object that connects to the system’s audio input.

`class AVAudioOutputNode`

An object that connects to the system’s audio output.

`class AVAudioIONode`

An object that performs audio input or output in the engine.

### Playback

Playing custom audio with your own player

Construct an audio player to play your custom audio data, and optionally take advantage of the advanced features of AirPlay 2.

Using voice processing

Add voice-processing capabilities to your app by using audio engine.

`class AVAudioPlayerNode`

An object for scheduling the playback of buffers or segments of audio files.

### MIDI

`class AVAudioSequencer`

An object that plays audio from a collection of MIDI events the system organizes into music tracks.

`class AVAudioUnitSampler`

An object that you configure with one or more instrument samples, based on Apple’s Sampler audio unit.

### Mixing

`class AVAudioMixerNode`

An object that takes any number of inputs and converts them into a single output.

`protocol AVAudioMixing`

A collection of properties that are applicable to the input bus of a mixer node.

### Effects

Creating custom audio effects

Add custom audio-effect processing to apps like Logic Pro X and GarageBand by creating Audio Unit (AU) plug-ins.

The data type for a plug-in component that provides audio processing or audio data generation.

### Rendering

Building a signal generator

Use an audio source node and a custom render call

Add offline audio processing features to your app by enabling offline manual rendering mode.

`class AVAudioSourceNode`

An object that supplies audio data.

`class AVAudioSinkNode`

An object that receives audio data.

### Conversion

`class AVAudioConverter`

An object that converts streams of audio between formats.

### Spatial audio

`class AVAudioEnvironmentNode`

An object that simulates a 3D audio environment.

`class AVAudioEnvironmentDistanceAttenuationParameters`

An object that specifies the amount of attenuation distance, the gradual loss in audio intensity, and other characteristics.

`class AVAudioEnvironmentReverbParameters`

A class that encapsulates the parameters that you use to control the reverb of the environment node class.

`protocol AVAudio3DMixing`

A collection of properties that define 3D mixing properties.

`struct AVAudio3DPoint`

A structure that represents a point in 3D space.

`struct AVAudio3DVectorOrientation`

A structure that represents two orthogonal vectors that describe the orientation of the listener in 3D space.

`struct AVAudio3DAngularOrientation`

A structure that represents the angular orientation of the listener in 3D space.

`enum AVAudio3DMixingSourceMode`

The source modes for the input bus of the audio environment node.

`enum AVAudio3DMixingRenderingAlgorithm`

The types of rendering algorithms available per input bus of the environment node.

`enum AVAudioEnvironmentOutputType`

The output types for using with the automatic 3D mixing rendering algorithm.

`enum AVAudio3DMixingPointSourceInHeadMode`

The in-head modes for a point source.

`typealias AVAudio3DVector`

A structure that represents a vector in 3D space, in degrees.

### Supporting data types

`class AVAudioBuffer`

An object that represents a buffer of audio data with a format.

`class AVAudioFile`

An object that represents an audio file that the system can open for reading or writing.

`class AVAudioTime`

An object you use to represent a moment in time.

Configure audio processing settings using standard key and value constants.

---

# https://developer.apple.com/documentation/avfaudio/speech-synthesis

Collection

- AVFAudio
- Speech synthesis

API Collection

# Speech synthesis

Configure voices to speak strings of text.

## Overview

The Speech Synthesis framework manages voice and speech synthesis, and requires two primary tasks:

Create an `AVSpeechUtterance` instance that contains the text to speak. Optionally, configure speech parameters, such as voice and rate, for each utterance.

// Create an utterance.
let utterance = AVSpeechUtterance(string: "The quick brown fox jumped over the lazy dog.")

// Configure the utterance.
utterance.rate = 0.57
utterance.pitchMultiplier = 0.8
utterance.postUtteranceDelay = 0.2
utterance.volume = 0.8

// Retrieve the British English voice.
let voice = AVSpeechSynthesisVoice(language: "en-GB")

// Assign the voice to the utterance.
utterance.voice = voice

Pass the utterance to an `AVSpeechSynthesizer` instance to produce spoken audio.

// Create a speech synthesizer.
let synthesizer = AVSpeechSynthesizer()

// Tell the synthesizer to speak the utterance.
synthesizer.speak(utterance)

Optionally, use the speech synthesizer instance to control or respond to ongoing speech; for example, assign its `delegate` to receive speech event notifications.

## Topics

### Spoken text attributes

`class AVSpeechUtterance`

An object that encapsulates the text for speech synthesis and parameters that affect the speech.

`class AVSpeechSynthesisVoice`

A distinct voice for use in speech synthesis.

### Speech synthesis controls

`class AVSpeechSynthesizer`

An object that produces synthesized speech from text utterances and enables monitoring or controlling of ongoing speech.

### Speech synthesis audio unit

`class AVSpeechSynthesisProviderAudioUnit`

An object that generates speech from text.

---

# https://developer.apple.com/documentation/avfaudio/macros

Collection

- AVFAudio
- Macros

API Collection

# Macros

## Topics

### Macros

`var AVAUDIOENGINE_HAVE_AUAUDIOUNIT: Int32`

`var AVAUDIOENGINE_HAVE_MUSICPLAYER: Int32`

`var AVAUDIOFORMAT_HAVE_CMFORMATDESCRIPTION: Int32`

`var AVAUDIOIONODE_HAVE_AUDIOUNIT: Int32`

`var AVAUDIONODE_HAVE_AUAUDIOUNIT: Int32`

`var AVAUDIOUNITCOMPONENT_HAVE_AUDIOCOMPONENT: Int32`

`var AVAUDIOUNIT_HAVE_AUDIOUNIT: Int32`

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessioncapability

- AVFAudio
- AVAudioSessionCapability Beta

Class

# AVAudioSessionCapability

Describes whether a specific capability is supported and if that capability is currently enabled

class AVAudioSessionCapability

## Topics

### Instance Properties

`var isEnabled: Bool`

A Boolean value that indicates whether the capability is enabled.

`var isSupported: Bool`

A Boolean value that indicates whether the capability is supported.

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`
- `Sendable`
- `SendableMetatype`

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionportextensionbluetoothmicrophone

- AVFAudio
- AVAudioSessionPortExtensionBluetoothMicrophone Beta

Class

# AVAudioSessionPortExtensionBluetoothMicrophone

An object that describes capabilities of Bluetooth microphone ports.

class AVAudioSessionPortExtensionBluetoothMicrophone

## Topics

### Instance Properties

`var highQualityRecording: AVAudioSessionCapability`

Describes whether this port supports Bluetooth high-quality recording.

## Relationships

### Inherits From

- `NSObject`

### Conforms To

- `CVarArg`
- `CustomDebugStringConvertible`
- `CustomStringConvertible`
- `Equatable`
- `Hashable`
- `NSObjectProtocol`
- `Sendable`
- `SendableMetatype`

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionspatialexperience-swift.protocol

- AVFAudio
- AVAudioSessionSpatialExperience

Protocol

# AVAudioSessionSpatialExperience

protocol AVAudioSessionSpatialExperience

## Topics

### Type Properties

`static var bypassed: AVAudioSession.BypassedSpatialExperience`

## Relationships

### Conforming Types

- `AVAudioSession.BypassedSpatialExperience`
- `AVAudioSession.FixedSpatialExperience`
- `AVAudioSession.HeadTrackedSpatialExperience`

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionsetactiveflags_notifyothersondeactivation

- AVFAudio
- AVAudioSessionSetActiveFlags\_NotifyOthersOnDeactivation Deprecated

Global Variable

# AVAudioSessionSetActiveFlags\_NotifyOthersOnDeactivation

A flag that indicates that when your audio session deactivates, any audio sessions that your audio session interrupted can reactivate themselves.

visionOS 1.0–1.0Deprecated

var AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation: Int { get }

## Discussion

This flag works when passed in the `flags` parameter of the `setActive(_:withFlags:)` instance method. You use this flag only when deactivating your audio session.

---

# https://developer.apple.com/documentation/avfaudio/avencoderaspfrequencykey

- AVFAudio
- AVEncoderASPFrequencyKey Beta

Global Variable

# AVEncoderASPFrequencyKey

let AVEncoderASPFrequencyKey: String

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avencodercontentsourcekey

- AVFAudio
- AVEncoderContentSourceKey Beta

Global Variable

# AVEncoderContentSourceKey

let AVEncoderContentSourceKey: String

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avencoderdynamicrangecontrolconfigurationkey

- AVFAudio
- AVEncoderDynamicRangeControlConfigurationKey Beta

Global Variable

# AVEncoderDynamicRangeControlConfigurationKey

let AVEncoderDynamicRangeControlConfigurationKey: String

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avsamplerateconverteralgorithm_mastering

- AVFAudio
- AVSampleRateConverterAlgorithm\_Mastering

Global Variable

# AVSampleRateConverterAlgorithm\_Mastering

The mastering encoder bit rate strategy.

let AVSampleRateConverterAlgorithm_Mastering: String

## See Also

### Algorithms

`let AVSampleRateConverterAlgorithm_Normal: String`

The usual encoder bit rate strategy.

`let AVSampleRateConverterAlgorithm_MinimumPhase: String`

The minimum phase encoder bit rate strategy.

---

# https://developer.apple.com/documentation/avfaudio/avsamplerateconverteralgorithm_minimumphase

- AVFAudio
- AVSampleRateConverterAlgorithm\_MinimumPhase

Global Variable

# AVSampleRateConverterAlgorithm\_MinimumPhase

The minimum phase encoder bit rate strategy.

let AVSampleRateConverterAlgorithm_MinimumPhase: String

## See Also

### Algorithms

`let AVSampleRateConverterAlgorithm_Normal: String`

The usual encoder bit rate strategy.

`let AVSampleRateConverterAlgorithm_Mastering: String`

The mastering encoder bit rate strategy.

---

# https://developer.apple.com/documentation/avfaudio/avsamplerateconverteralgorithm_normal

- AVFAudio
- AVSampleRateConverterAlgorithm\_Normal

Global Variable

# AVSampleRateConverterAlgorithm\_Normal

The usual encoder bit rate strategy.

let AVSampleRateConverterAlgorithm_Normal: String

## See Also

### Algorithms

`let AVSampleRateConverterAlgorithm_MinimumPhase: String`

The minimum phase encoder bit rate strategy.

`let AVSampleRateConverterAlgorithm_Mastering: String`

The mastering encoder bit rate strategy.

---

# https://developer.apple.com/documentation/avfaudio/avmakebeatrange(_:_:)

#app-main)

- AVFAudio
- AVMakeBeatRange(\_:\_:)

Function

# AVMakeBeatRange(\_:\_:)

Creates a beat range with the specified start time and length.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

func AVMakeBeatRange(
_ startBeat: AVMusicTimeStamp,
_ lengthInBeats: AVMusicTimeStamp

## Parameters

`startBeat`

The timestamp for the start position.

`lengthInBeats`

The length of the beat range, in beats.

---

# https://developer.apple.com/documentation/avfaudio/avaudioconverterinputblock

- AVFAudio
- AVAudioConverterInputBlock

Type Alias

# AVAudioConverterInputBlock

A block to get input data for conversion, as necessary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

---

# https://developer.apple.com/documentation/avfaudio/avbeatrange-swift.typealias

- AVFAudio
- AVBeatRange

Type Alias

# AVBeatRange

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

typealias AVBeatRange = _AVBeatRange

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Sendable`

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayercompletionhandler

- AVFAudio
- AVMIDIPlayerCompletionHandler

Type Alias

# AVMIDIPlayerCompletionHandler

A callback the system invokes when MIDI playback completes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

---

# https://developer.apple.com/documentation/avfaudio/avaudiocontentsource

- AVFAudio
- AVAudioContentSource Beta

Enumeration

# AVAudioContentSource

enum AVAudioContentSource

## Topics

### Enumeration Cases

`case appleAV_Spatial_Live`

`case appleAV_Spatial_Offline`

`case appleAV_Traditional_Live`

`case appleAV_Traditional_Offline`

`case appleCapture_Spatial`

`case appleCapture_Spatial_Enhanced`

`case appleCapture_Traditional`

`case appleMusic_Spatial`

`case appleMusic_Traditional`

`case applePassthrough`

`case av_Spatial_Live`

`case av_Spatial_Offline`

`case av_Traditional_Live`

`case av_Traditional_Offline`

`case capture_Spatial`

`case capture_Spatial_Enhanced`

`case capture_Traditional`

`case music_Spatial`

`case music_Traditional`

`case passthrough`

`case reserved`

`case unspecified`

### Initializers

`init?(rawValue: Int)`

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `Hashable`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avaudiodynamicrangecontrolconfiguration

- AVFAudio
- AVAudioDynamicRangeControlConfiguration

Enumeration

# AVAudioDynamicRangeControlConfiguration

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

enum AVAudioDynamicRangeControlConfiguration

## Topics

### Enumeration Cases

`case capture`

`case movie`

`case music`

`case none`

`case speech`

### Initializers

`init?(rawValue: Int)`

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `Hashable`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`

---

# https://developer.apple.com/documentation/avfaudio/handling-audio-interruptions)



---

# https://developer.apple.com/documentation/avfaudio/responding-to-audio-route-changes)



---

# https://developer.apple.com/documentation/avfaudio/adding-synthesized-speech-to-calls)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/capturing-stereo-audio-from-built-in-microphones)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession)



---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication)



---

# https://developer.apple.com/documentation/avfaudio/avaudioroutingarbiter)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer)



---

# https://developer.apple.com/documentation/avfaudio/avaudiorecorder)



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer)



---

# https://developer.apple.com/documentation/avfaudio/audio-engine)



---

# https://developer.apple.com/documentation/avfaudio/speech-synthesis)



---

# https://developer.apple.com/documentation/avfaudio/macros)



---

# https://developer.apple.com/documentation/avfaudio/avaudiosessioncapability)



---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionportextensionbluetoothmicrophone)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionspatialexperience-swift.protocol)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionsetactiveflags_notifyothersondeactivation)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avencoderaspfrequencykey)



---

# https://developer.apple.com/documentation/avfaudio/avencodercontentsourcekey)



---

# https://developer.apple.com/documentation/avfaudio/avencoderdynamicrangecontrolconfigurationkey)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avsamplerateconverteralgorithm_mastering)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avsamplerateconverteralgorithm_minimumphase)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avsamplerateconverteralgorithm_normal)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avmakebeatrange(_:_:))



---

# https://developer.apple.com/documentation/avfaudio/avaudioconverterinputblock)



---

# https://developer.apple.com/documentation/avfaudio/avbeatrange-swift.typealias)



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayercompletionhandler)



---

# https://developer.apple.com/documentation/avfaudio/avaudiocontentsource)



---

# https://developer.apple.com/documentation/avfaudio/avaudiodynamicrangecontrolconfiguration)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/overridemutedmicrophoneinterruption

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- overrideMutedMicrophoneInterruption

Type Property

# overrideMutedMicrophoneInterruption

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions { get }

## Mentioned in

Handling audio interruptions

## Discussion

Some devices include a privacy feature that mutes the built-in microphone at the hardware level in certain conditions, such as when you close the Smart Folio cover of an iPad. When this occurs, the system interrupts the audio session that’s capturing input from the microphone. Attempting to start audio input after the system mutes the microphone results in an error.

If your app uses an audio session category that supports input and output, such as `playAndRecord`, you can set this option to disable the default behavior and continue using the session. Disabling the default behavior may be useful to allow your app to continue playback when recording or monitoring a muted microphone doesn’t lead to a poor user experience. When you set this option, playback continues as normal, and the microphone hardware produces sample buffers, but with values of `0`.

## See Also

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setprefersnointerruptionsfromsystemalerts(_:)

#app-main)

- AVFAudio
- AVAudioSession
- setPrefersNoInterruptionsFromSystemAlerts(\_:)

Instance Method

# setPrefersNoInterruptionsFromSystemAlerts(\_:)

Sets the preference for not interrupting the audio session with system alerts.

func setPrefersNoInterruptionsFromSystemAlerts(_ inValue: Bool) throws

## Parameters

`inValue`

The interruption preference value.

## Mentioned in

Handling audio interruptions

## Discussion

Beginning in iOS 14, users can set a global preference that indicates whether the system displays incoming calls using a banner or a full-screen display style. If using the banner style, setting this value to `true` prevents the system from interrupting the audio session with incoming call notifications, and gives the user an opportunity to accept or decline the call. The system only interrupts the audio session if the user accepts the call.

Enabling this preference can improve the user experience of apps with audio sessions that you don’t want to interrupt, such as those that record audiovisual media or that you use for music performance.

## See Also

### Handling interruptions

`var prefersNoInterruptionsFromSystemAlerts: Bool`

A Boolean value that indicates a preference for not interrupting the session with system alerts.

`var prefersInterruptionOnRouteDisconnect: Bool`

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

`func setPrefersInterruptionOnRouteDisconnect(Bool) throws`

Sets a preference to interrupt the audio session when the active route disconnects.

`class let interruptionNotification: NSNotification.Name`

A notification the system posts when an audio interruption occurs.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptionnotification

- AVFAudio
- AVAudioSession
- interruptionNotification

Type Property

# interruptionNotification

A notification the system posts when an audio interruption occurs.

class let interruptionNotification: NSNotification.Name

## Mentioned in

Handling audio interruptions

## Discussion

The notification’s user-information dictionary contains the `AVAudioSessionInterruptionTypeKey` key. If the interruption type is `AVAudioSession.InterruptionType.began`, the system interrupted your app’s audio session and it’s no longer active. If the interruption type is `AVAudioSession.InterruptionType.ended`, this dictionary also contains the `AVAudioSessionInterruptionOptionKey` key.

See Handling audio interruptions for more information on using this notification.

The system posts this notification on the main thread.

## Topics

### User Info Keys

`let AVAudioSessionInterruptionTypeKey: String`

A user info key to retrieve the interruption type.

`let AVAudioSessionInterruptionOptionKey: String`

A user info key to retrieve the interruption option.

`let AVAudioSessionInterruptionReasonKey: String`

A user info key to retrieve the interruption reason.

`let AVAudioSessionInterruptionWasSuspendedKey: String`

A user info key used to determine if the interruption is due to the audio session being deactivated when the system suspended the app.

Deprecated

### User Info Values

`enum InterruptionType`

Constants that describe the type of an audio interruption.

`struct InterruptionOptions`

Constants that indicate the state of an audio session after an interruption.

`enum InterruptionReason`

Constants that define the reasons for an audio session interruption.

## See Also

### Handling interruptions

`var prefersNoInterruptionsFromSystemAlerts: Bool`

A Boolean value that indicates a preference for not interrupting the session with system alerts.

`func setPrefersNoInterruptionsFromSystemAlerts(Bool) throws`

Sets the preference for not interrupting the audio session with system alerts.

`var prefersInterruptionOnRouteDisconnect: Bool`

A Boolean value that indicates whether the system interrupts the audio session when the active route disconnects.

`func setPrefersInterruptionOnRouteDisconnect(Bool) throws`

Sets a preference to interrupt the audio session when the active route disconnects.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptiontype

- AVFAudio
- AVAudioSession
- AVAudioSession.InterruptionType

Enumeration

# AVAudioSession.InterruptionType

Constants that describe the type of an audio interruption.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

enum InterruptionType

## Mentioned in

Handling audio interruptions

## Topics

### Interruption Types

`case began`

A type that indicates that the operating system began interrupting the audio session.

`case ended`

A type that indicates that the operating system ended interrupting the audio session.

### Initializers

`init?(rawValue: UInt)`

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `Hashable`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`

## See Also

### User Info Values

`struct InterruptionOptions`

Constants that indicate the state of an audio session after an interruption.

`enum InterruptionReason`

Constants that define the reasons for an audio session interruption.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptiontype/ended

- AVFAudio
- AVAudioSession
- AVAudioSession.InterruptionType
- AVAudioSession.InterruptionType.ended

Case

# AVAudioSession.InterruptionType.ended

A type that indicates that the operating system ended interrupting the audio session.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

case ended

## Mentioned in

Handling audio interruptions

## See Also

### Interruption Types

`case began`

A type that indicates that the operating system began interrupting the audio session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptionoptions

- AVFAudio
- AVAudioSession
- AVAudioSession.InterruptionOptions

Structure

# AVAudioSession.InterruptionOptions

Constants that indicate the state of an audio session after an interruption.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

struct InterruptionOptions

## Mentioned in

Handling audio interruptions

## Topics

### Creating an Interruption Option

`init(rawValue: UInt)`

Creates a new instance with the raw value you specify.

### Getting Standard Interruption Options

`static var shouldResume: AVAudioSession.InterruptionOptions`

An option that indicates the interruption by another audio session has ended and the app can resume its audio session.

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `ExpressibleByArrayLiteral`
- `OptionSet`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`
- `SetAlgebra`

## See Also

### User Info Values

`enum InterruptionType`

Constants that describe the type of an audio interruption.

`enum InterruptionReason`

Constants that define the reasons for an audio session interruption.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/overridemutedmicrophoneinterruption)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setprefersnointerruptionsfromsystemalerts(_:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptionnotification).

.#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptiontype)



---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptiontype/ended),

,#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/interruptionoptions)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/init(contentsof:soundbankurl:)



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/init(data:soundbankurl:)

#app-main)

- AVFAudio
- AVMIDIPlayer
- init(data:soundBankURL:)

Initializer

# init(data:soundBankURL:)

Creates a player to play MIDI data with the specified soundbank.

init(
data: Data,
soundBankURL bankURL: URL?
) throws

## Parameters

`data`

The data to play.

`bankURL`

The URL of the sound bank. The sound bank must be a SoundFont2 or DLS bank. In macOS, you can pass `nil` for the bank URL argument to use the default sound bank. In iOS, you must always pass a valid bank file.

## Return Value

A new MIDI player, or `nil` if an error occurred.

## See Also

### Creating a MIDI player

`init(contentsOf: URL, soundBankURL: URL?) throws`

Creates a player to play a MIDI file with the specified soundbank.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/preparetoplay()

#app-main)

- AVFAudio
- AVMIDIPlayer
- prepareToPlay()

Instance Method

# prepareToPlay()

Prepares the player to play the sequence by prerolling all events.

func prepareToPlay()

## Discussion

The system automatically calls this method on playback, but calling it in advance minimizes the delay between calling `play(_:)` and the start of sound output.

## See Also

### Controlling playback

Plays the MIDI sequence.

`func stop()`

Stops playing the sequence.

`var isPlaying: Bool`

A Boolean value that indicates whether the sequence is playing.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/play(_:)

#app-main)

- AVFAudio
- AVMIDIPlayer
- play(\_:)

Instance Method

# play(\_:)

Plays the MIDI sequence.

func play() async

## Parameters

`completionHandler`

A closure the system calls when playback completes.

## Topics

### Closures

`typealias AVMIDIPlayerCompletionHandler`

A callback the system invokes when MIDI playback completes.

## See Also

### Controlling playback

`func prepareToPlay()`

Prepares the player to play the sequence by prerolling all events.

`func stop()`

Stops playing the sequence.

`var isPlaying: Bool`

A Boolean value that indicates whether the sequence is playing.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/stop()



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/isplaying

- AVFAudio
- AVMIDIPlayer
- isPlaying

Instance Property

# isPlaying

A Boolean value that indicates whether the sequence is playing.

var isPlaying: Bool { get }

## See Also

### Controlling playback

`func prepareToPlay()`

Prepares the player to play the sequence by prerolling all events.

Plays the MIDI sequence.

`func stop()`

Stops playing the sequence.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/rate

- AVFAudio
- AVMIDIPlayer
- rate

Instance Property

# rate

The playback rate of the player.

var rate: Float { get set }

## Discussion

The default value is `1.0,` the standard playback rate.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/currentposition

- AVFAudio
- AVMIDIPlayer
- currentPosition

Instance Property

# currentPosition

The current playback position, in seconds.

var currentPosition: TimeInterval { get set }

## See Also

### Accessing player timing

`var duration: TimeInterval`

The duration, in seconds, of the currently loaded file.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/duration

- AVFAudio
- AVMIDIPlayer
- duration

Instance Property

# duration

The duration, in seconds, of the currently loaded file.

var duration: TimeInterval { get }

## See Also

### Accessing player timing

`var currentPosition: TimeInterval`

The current playback position, in seconds.

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/init(contentsof:soundbankurl:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/init(data:soundbankurl:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/preparetoplay())



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/play(_:))



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/stop())



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/isplaying)



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/rate)



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/currentposition)



---

# https://developer.apple.com/documentation/avfaudio/avmidiplayer/duration)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(contentsof:)

#app-main)

- AVFAudio
- AVAudioPlayer
- init(contentsOf:)

Initializer

# init(contentsOf:)

Creates a player to play audio from a file.

init(contentsOf url: URL) throws

## Parameters

`url`

A URL that identifies the local audio file to play.

## Return Value

A new audio player instance, or `nil` if an error occurs.

## Discussion

The audio data must be in a format that Core Audio supports.

## See Also

### Creating an audio player

`init(contentsOf: URL, fileTypeHint: String?) throws`

Creates a player to play audio from a file of a particular type.

`init(data: Data) throws`

Creates a player to play in-memory audio data.

`init(data: Data, fileTypeHint: String?) throws`

Creates a player to play in-memory audio data of a particular type.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(contentsof:filetypehint:)

#app-main)

- AVFAudio
- AVAudioPlayer
- init(contentsOf:fileTypeHint:)

Initializer

# init(contentsOf:fileTypeHint:)

Creates a player to play audio from a file of a particular type.

init(
contentsOf url: URL,
fileTypeHint utiString: String?
) throws

## Parameters

`url`

A URL that identifies the local audio file to play.

`utiString`

The uniform type identifier (UTI) string of the file format.

## Return Value

A new audio player instance, or `nil` if there is an error.

## Discussion

The audio data must be in a format that Core Audio supports. Passing a file type hint helps the system parse the data if it can’t determine the file type or if the data is corrupt. See `AVFileType` for supported values.

## See Also

### Creating an audio player

`init(contentsOf: URL) throws`

Creates a player to play audio from a file.

`init(data: Data) throws`

Creates a player to play in-memory audio data.

`init(data: Data, fileTypeHint: String?) throws`

Creates a player to play in-memory audio data of a particular type.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(data:)

#app-main)

- AVFAudio
- AVAudioPlayer
- init(data:)

Initializer

# init(data:)

Creates a player to play in-memory audio data.

init(data: Data) throws

## Parameters

`data`

A buffer with the audio data to play.

## Return Value

A new audio player instance, or `nil` if an error occurs.

## Discussion

The audio data must be in a format that Core Audio supports.

## See Also

### Creating an audio player

`init(contentsOf: URL) throws`

Creates a player to play audio from a file.

`init(contentsOf: URL, fileTypeHint: String?) throws`

Creates a player to play audio from a file of a particular type.

`init(data: Data, fileTypeHint: String?) throws`

Creates a player to play in-memory audio data of a particular type.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(data:filetypehint:)

#app-main)

- AVFAudio
- AVAudioPlayer
- init(data:fileTypeHint:)

Initializer

# init(data:fileTypeHint:)

Creates a player to play in-memory audio data of a particular type.

init(
data: Data,
fileTypeHint utiString: String?
) throws

## Parameters

`data`

A buffer with the audio data to play.

`utiString`

The uniform type identifier (UTI) string of the file format.

## Return Value

A new audio player instance, or `nil` if an error occurs.

## Discussion

The audio data must be in a format that Core Audio supports. Passing a file type hint helps the system parse the data if it can’t determine the file type or if the data is corrupt. See `AVFileType` for supported values.

## See Also

### Creating an audio player

`init(contentsOf: URL) throws`

Creates a player to play audio from a file.

`init(contentsOf: URL, fileTypeHint: String?) throws`

Creates a player to play audio from a file of a particular type.

`init(data: Data) throws`

Creates a player to play in-memory audio data.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/preparetoplay()

#app-main)

- AVFAudio
- AVAudioPlayer
- prepareToPlay()

Instance Method

# prepareToPlay()

Prepares the player for audio playback.

## Return Value

`true` if the system successfully prepares the player; otherwise, `false`.

## Discussion

Calling this method preloads audio buffers and acquires the audio hardware necessary for playback. This method activates the audio session, so pass `false` to `setActive:error:` if immediate playback isn’t necessary. For example, when using the category option `duckOthers`, this method lowers the audio outside of the app.

The system calls this method when using the method `play()`, but calling it in advance minimizes the delay between calling `play()` and the start of sound output.

Calling `stop()`, or allowing a sound to finish playing, undoes this setup.

## See Also

### Controlling playback

Plays audio asynchronously.

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

`func pause()`

Pauses audio playback.

`func stop()`

Stops playback and undoes the setup the system requires for playback.

`var isPlaying: Bool`

A Boolean value that indicates whether the player is currently playing audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/play()

#app-main)

- AVFAudio
- AVAudioPlayer
- play()

Instance Method

# play()

Plays audio asynchronously.

## Return Value

`true` if playback starts successfully; otherwise, `false`.

## Discussion

Calling this method implicitly calls `prepareToPlay()` if the audio player is unprepared for playback.

## See Also

### Controlling playback

Prepares the player for audio playback.

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

`func pause()`

Pauses audio playback.

`func stop()`

Stops playback and undoes the setup the system requires for playback.

`var isPlaying: Bool`

A Boolean value that indicates whether the player is currently playing audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/play(attime:)

#app-main)

- AVFAudio
- AVAudioPlayer
- play(atTime:)

Instance Method

# play(atTime:)

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

## Parameters

`time`

The audio device time to begin playback. This time must be later than the device’s current time.

## Return Value

`true` if playback starts successfully; otherwise, `false`.

## Discussion

Use this method to precisely synchronize the playback of two or more audio player objects as the following example shows:

func startSynchronizedPlayback() {
// Create a time offset relative to the current device time.
let timeOffset = playerOne.deviceCurrentTime + 0.01

// Start playback of both players at the same time.
playerOne.play(atTime: timeOffset)
playerTwo.play(atTime: timeOffset)
}

Calling this method implicitly calls `prepareToPlay()` if the audio player is unprepared for playback.

## See Also

### Controlling playback

Prepares the player for audio playback.

Plays audio asynchronously.

`func pause()`

Pauses audio playback.

`func stop()`

Stops playback and undoes the setup the system requires for playback.

`var isPlaying: Bool`

A Boolean value that indicates whether the player is currently playing audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/pause()

#app-main)

- AVFAudio
- AVAudioPlayer
- pause()

Instance Method

# pause()

Pauses audio playback.

func pause()

## Discussion

Unlike calling `stop()`, pausing playback doesn’t deallocate hardware resources. It leaves the audio ready to resume playback from where it stops.

## See Also

### Controlling playback

Prepares the player for audio playback.

Plays audio asynchronously.

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

`func stop()`

Stops playback and undoes the setup the system requires for playback.

`var isPlaying: Bool`

A Boolean value that indicates whether the player is currently playing audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/stop()

#app-main)

- AVFAudio
- AVAudioPlayer
- stop()

Instance Method

# stop()

Stops playback and undoes the setup the system requires for playback.

func stop()

## Discussion

Calling this method undoes the resource allocation the system performs in `prepareToPlay()` or `play()`. It doesn’t reset the player’s `currentTime` value to `0`, so playback resumes from where it stops.

## See Also

### Controlling playback

Prepares the player for audio playback.

Plays audio asynchronously.

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

`func pause()`

Pauses audio playback.

`var isPlaying: Bool`

A Boolean value that indicates whether the player is currently playing audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/isplaying

- AVFAudio
- AVAudioPlayer
- isPlaying

Instance Property

# isPlaying

A Boolean value that indicates whether the player is currently playing audio.

var isPlaying: Bool { get }

## See Also

### Controlling playback

Prepares the player for audio playback.

Plays audio asynchronously.

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

`func pause()`

Pauses audio playback.

`func stop()`

Stops playback and undoes the setup the system requires for playback.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/volume

- AVFAudio
- AVAudioPlayer
- volume

Instance Property

# volume

The audio player’s volume relative to other audio output.

var volume: Float { get set }

## Discussion

This property supports values ranging from `0.0` for silence to `1.0` for full volume.

## See Also

### Configuring playback settings

`func setVolume(Float, fadeDuration: TimeInterval)`

Changes the audio player’s volume over a duration of time.

`var pan: Float`

The audio player’s stereo pan position.

`var enableRate: Bool`

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

`var rate: Float`

The audio player’s playback rate.

`var numberOfLoops: Int`

The number of times the audio repeats playback.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/setvolume(_:fadeduration:)

#app-main)

- AVFAudio
- AVAudioPlayer
- setVolume(\_:fadeDuration:)

Instance Method

# setVolume(\_:fadeDuration:)

Changes the audio player’s volume over a duration of time.

func setVolume(
_ volume: Float,
fadeDuration duration: TimeInterval
)

## Parameters

`volume`

The target volume.

`duration`

The duration, in seconds, over which to fade the volume.

## See Also

### Configuring playback settings

`var volume: Float`

The audio player’s volume relative to other audio output.

`var pan: Float`

The audio player’s stereo pan position.

`var enableRate: Bool`

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

`var rate: Float`

The audio player’s playback rate.

`var numberOfLoops: Int`

The number of times the audio repeats playback.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/pan

- AVFAudio
- AVAudioPlayer
- pan

Instance Property

# pan

The audio player’s stereo pan position.

var pan: Float { get set }

## Discussion

Set this property value to position the audio in the stereo field. Use a value of `-1.0` to indicate full left, `1.0` for full right, and `0.0` for center.

## See Also

### Configuring playback settings

`var volume: Float`

The audio player’s volume relative to other audio output.

`func setVolume(Float, fadeDuration: TimeInterval)`

Changes the audio player’s volume over a duration of time.

`var enableRate: Bool`

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

`var rate: Float`

The audio player’s playback rate.

`var numberOfLoops: Int`

The number of times the audio repeats playback.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/enablerate

- AVFAudio
- AVAudioPlayer
- enableRate

Instance Property

# enableRate

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

var enableRate: Bool { get set }

## Discussion

To enable modifying the player’s rate, set this property to `true` after you create the player, but before you call `prepareToPlay()`.

## See Also

### Configuring playback settings

`var volume: Float`

The audio player’s volume relative to other audio output.

`func setVolume(Float, fadeDuration: TimeInterval)`

Changes the audio player’s volume over a duration of time.

`var pan: Float`

The audio player’s stereo pan position.

`var rate: Float`

The audio player’s playback rate.

`var numberOfLoops: Int`

The number of times the audio repeats playback.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/rate

- AVFAudio
- AVAudioPlayer
- rate

Instance Property

# rate

The audio player’s playback rate.

var rate: Float { get set }

## Discussion

To set an audio player’s playback rate, you must first enable the rate adjustment by setting its `enableRate` property to `true`.

The default value of this property is `1.0`, which indicates that audio playback occurs at standard speed. This property supports values in the range of `0.5` for half-speed play

### Configuring playback settings

`var volume: Float`

The audio player’s volume relative to other audio output.

`func setVolume(Float, fadeDuration: TimeInterval)`

Changes the audio player’s volume over a duration of time.

`var pan: Float`

The audio player’s stereo pan position.

`var enableRate: Bool`

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

`var numberOfLoops: Int`

The number of times the audio repeats playback.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/numberofloops



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/currenttime

- AVFAudio
- AVAudioPlayer
- currentTime

Instance Property

# currentTime

The current playback time, in seconds, within the audio timeline.

var currentTime: TimeInterval { get set }

## Discussion

If the sound is playing, this property value is the offset, in seconds, from the start of the sound. If the sound isn’t playing, this property indicates the offset from where playback starts upon calling the `play()` method.

Use this property to seek to a specific time in the audio data or to implement audio fast-forward and rewind functions.

## See Also

### Accessing player timing

`var duration: TimeInterval`

The total duration, in seconds, of the player’s audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/duration

- AVFAudio
- AVAudioPlayer
- duration

Instance Property

# duration

The total duration, in seconds, of the player’s audio.

var duration: TimeInterval { get }

## See Also

### Accessing player timing

`var currentTime: TimeInterval`

The current playback time, in seconds, within the audio timeline.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/numberofchannels

- AVFAudio
- AVAudioPlayer
- numberOfChannels

Instance Property

# numberOfChannels

The number of audio channels in the player’s audio.

var numberOfChannels: Int { get }

## See Also

### Managing audio channels

[`var channelAssignments: [AVAudioSessionChannelDescription]?`](https://developer.apple.com/documentation/avfaudio/avaudioplayer/channelassignments)

An array of channel descriptions for the audio player.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/ismeteringenabled

- AVFAudio
- AVAudioPlayer
- isMeteringEnabled

Instance Property

# isMeteringEnabled

A Boolean value that indicates whether the player is able to generate audio-level metering data.

var isMeteringEnabled: Bool { get set }

## Discussion

By default, the player doesn’t generate audio-level metering data. Because metering uses computing resources, enable it only if you intend to use it.

## See Also

### Managing audio-level metering

`func updateMeters()`

Refreshes the average and peak power values for all channels of an audio player.

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/updatemeters()



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/averagepower(forchannel:)

#app-main)

- AVFAudio
- AVAudioPlayer
- averagePower(forChannel:)

Instance Method

# averagePower(forChannel:)

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

## Parameters

`channelNumber`

The audio channel with the average power value you want to retrieve. Channel numbers are zero-indexed. A monaural signal, or the left channel of a stereo signal, has channel number `0`.

## Return Value

A floating-point value, in dBFS, that indicates the audio channel’s current average power.

## Discussion

Before asking the player for its average power value, you must call `updateMeters()` to generate the latest data. The returned value ranges from `–160` dBFS, indicating minimum power, to 0 dBFS, indicating maximum power.

## See Also

### Managing audio-level metering

`var isMeteringEnabled: Bool`

A Boolean value that indicates whether the player is able to generate audio-level metering data.

`func updateMeters()`

Refreshes the average and peak power values for all channels of an audio player.

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/peakpower(forchannel:)

#app-main)

- AVFAudio
- AVAudioPlayer
- peakPower(forChannel:)

Instance Method

# peakPower(forChannel:)

Returns the peak power, in decibels full-scale (dBFS), for an audio channel.

## Parameters

`channelNumber`

The audio channel with the peak power value you want to obtain. Channel numbers are zero-indexed. A monaural signal, or the left channel of a stereo signal, has channel number `0`.

## Return Value

A floating-point value, in dBFS, that indicates the audio channel’s current peak power.

## Discussion

Before asking the player for its peak power value, you must call `updateMeters()` to generate the latest data. The returned value ranges from `–160` dBFS, indicating minimum power, to 0 dBFS, indicating maximum power.

## See Also

### Managing audio-level metering

`var isMeteringEnabled: Bool`

A Boolean value that indicates whether the player is able to generate audio-level metering data.

`func updateMeters()`

Refreshes the average and peak power values for all channels of an audio player.

Returns the average power, in decibels full-scale (dBFS), for an audio channel.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/delegate

- AVFAudio
- AVAudioPlayer
- delegate

Instance Property

# delegate

The delegate object for the audio player.

weak var delegate: (any AVAudioPlayerDelegate)? { get set }

## See Also

### Responding to player events

`protocol AVAudioPlayerDelegate`

A protocol that defines the methods to respond to audio playback events and decoding errors.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayerdelegate



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/url

- AVFAudio
- AVAudioPlayer
- url

Instance Property

# url

The URL of the audio file.

var url: URL? { get }

## Discussion

This property is `nil` if you don’t create the player with a URL.

## See Also

### Inspecting the audio data

`var data: Data?`

The audio data associated with the player.

`var format: AVAudioFormat`

The format of the player’s audio data.

[`var settings: [String : Any]`](https://developer.apple.com/documentation/avfaudio/avaudioplayer/settings)

A dictionary that provides information about the player’s audio data.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/data

- AVFAudio
- AVAudioPlayer
- data

Instance Property

# data

The audio data associated with the player.

var data: Data? { get }

## Discussion

This property is `nil` if you don’t create the player with a data buffer.

## See Also

### Inspecting the audio data

`var url: URL?`

The URL of the audio file.

`var format: AVAudioFormat`

The format of the player’s audio data.

[`var settings: [String : Any]`](https://developer.apple.com/documentation/avfaudio/avaudioplayer/settings)

A dictionary that provides information about the player’s audio data.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/format

- AVFAudio
- AVAudioPlayer
- format

Instance Property

# format

The format of the player’s audio data.

var format: AVAudioFormat { get }

## See Also

### Inspecting the audio data

`var url: URL?`

The URL of the audio file.

`var data: Data?`

The audio data associated with the player.

[`var settings: [String : Any]`](https://developer.apple.com/documentation/avfaudio/avaudioplayer/settings)

A dictionary that provides information about the player’s audio data.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/currentdevice

- AVFAudio
- AVAudioPlayer
- currentDevice

Instance Property

# currentDevice

The unique identifier of the current audio player.

var currentDevice: String? { get set }

## See Also

### Accessing device information

`var deviceCurrentTime: TimeInterval`

The time value, in seconds, of the audio output device’s clock.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/devicecurrenttime

- AVFAudio
- AVAudioPlayer
- deviceCurrentTime

Instance Property

# deviceCurrentTime

The time value, in seconds, of the audio output device’s clock.

var deviceCurrentTime: TimeInterval { get }

## Discussion

The value of this property increases monotonically while an audio player is playing or is in a paused state. If you connect more than one audio player to the audio output device, the time continues incrementing while at least one of the players is playing or is in a paused state. If the audio output device has no connected audio players that are either playing or are in a paused state, device time reverts to `0.0`.

## See Also

### Accessing device information

`var currentDevice: String?`

The unique identifier of the current audio player.

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/intendedspatialexperience-27klj

- AVFAudio
- AVAudioPlayer
- intendedSpatialExperience Beta

Instance Property

# intendedSpatialExperience

The AVAudioPlayer’s intended spatial experience.

var intendedSpatialExperience: any SpatialAudioExperience { get set }

## Discussion

The default value of .automatic means the player uses its AVAudioSession’s intended spatial experience. See CASpatialAudioExperience for more details.

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(contentsof:))



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(contentsof:filetypehint:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(data:))



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/init(data:filetypehint:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/preparetoplay())



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/play())



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/play(attime:))



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/pause())



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/stop())



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/isplaying)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/volume)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/setvolume(_:fadeduration:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/pan)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/enablerate)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/rate)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/numberofloops)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/currenttime)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/duration)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/numberofchannels)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/channelassignments)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/ismeteringenabled)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/updatemeters())



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/averagepower(forchannel:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/peakpower(forchannel:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/delegate)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayerdelegate)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/url)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/data)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/format)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/settings)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/currentdevice)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/devicecurrenttime)



---

# https://developer.apple.com/documentation/avfaudio/avaudioplayer/intendedspatialexperience-27klj)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/servicedisabled

- AVFAudio
- AVAudioApplication
- AVAudioApplication.MicrophoneInjectionPermission
- AVAudioApplication.MicrophoneInjectionPermission.serviceDisabled

Case

# AVAudioApplication.MicrophoneInjectionPermission.serviceDisabled

A person disables this service for all apps.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

case serviceDisabled

## See Also

### Permissions

`case undetermined`

The app hasn’t requested a person’s permission to add audio to calls.

`case granted`

A person grants the app permission to add audio to calls.

`case denied`

A person denies the app permission to add audio to calls.

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/undetermined

- AVFAudio
- AVAudioApplication
- AVAudioApplication.MicrophoneInjectionPermission
- AVAudioApplication.MicrophoneInjectionPermission.undetermined

Case

# AVAudioApplication.MicrophoneInjectionPermission.undetermined

The app hasn’t requested a person’s permission to add audio to calls.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

case undetermined

## See Also

### Permissions

`case serviceDisabled`

A person disables this service for all apps.

`case granted`

A person grants the app permission to add audio to calls.

`case denied`

A person denies the app permission to add audio to calls.

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/requestrecordpermission(completionhandler:)

#app-main)

- AVFAudio
- AVAudioApplication
- requestRecordPermission(completionHandler:)

Type Method

# requestRecordPermission(completionHandler:)

Determines whether the app has permission to record audio.

## Parameters

`response`

A Boolean value that indicates whether the user grants the app permission to record audio.

## Discussion

Recording audio requires explicit permission from the user. The first time your app attempts to record audio input, the system automatically prompts the user for permission. You can also explicitly ask for permission by calling this method. This method returns immediately, but the system waits for user input if the user hasn’t previously granted or denied recording permission.

// Request permission to record.
if await AVAudioApplication.requestRecordPermission() {
// The user grants access. Present recording interface.
} else {
// The user denies access. Present a message that indicates
// that they can change their permission settings in the
// Privacy & Security section of the Settings app.
}

Unless a user grants your app permission to record audio, it captures only silence (zeroed out audio samples).

After a user responds to a recording permission prompt from your app, the system remembers their choice and won’t prompt them again. If a user denies the app recording permission, they can grant it access in the Privacy & Security section of the Settings app.

## See Also

### Requesting audio recording permission

`var recordPermission: AVAudioApplication.recordPermission`

The app’s permission to record audio.

`enum recordPermission`

Constants that indicate the app’s permission to record audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/granted



---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/denied

- AVFAudio
- AVAudioApplication
- AVAudioApplication.MicrophoneInjectionPermission
- AVAudioApplication.MicrophoneInjectionPermission.denied

Case

# AVAudioApplication.MicrophoneInjectionPermission.denied

A person denies the app permission to add audio to calls.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

case denied

## See Also

### Permissions

`case serviceDisabled`

A person disables this service for all apps.

`case undetermined`

The app hasn’t requested a person’s permission to add audio to calls.

`case granted`

A person grants the app permission to add audio to calls.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setpreferredmicrophoneinjectionmode(_:)

#app-main)

- AVFAudio
- AVAudioSession
- setPreferredMicrophoneInjectionMode(\_:)

Instance Method

# setPreferredMicrophoneInjectionMode(\_:)

Sets the preferred mode of injecting audio into another app’s input stream.

func setPreferredMicrophoneInjectionMode(_ inValue: AVAudioSession.MicrophoneInjectionMode) throws

## Parameters

`inValue`

The preferred microphone injection mode.

## See Also

### Enabling adding audio to calls

`var isMicrophoneInjectionAvailable: Bool`

A Boolean value that indicates whether microphone injection is available.

`var preferredMicrophoneInjectionMode: AVAudioSession.MicrophoneInjectionMode`

The preferred mode of injecting audio into another app’s input stream.

`enum MicrophoneInjectionMode`

The modes of injecting audio into another app’s input stream.

`class let microphoneInjectionCapabilitiesChangeNotification: NSNotification.Name`

A notification the system posts when its capability to inject audio into an input stream changes.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/microphoneinjectionmode/spokenaudio

- AVFAudio
- AVAudioSession
- AVAudioSession.MicrophoneInjectionMode
- AVAudioSession.MicrophoneInjectionMode.spokenAudio

Case

# AVAudioSession.MicrophoneInjectionMode.spokenAudio

A mode that indicates to inject spoken audio, like synthesized speech, along with microphone audio.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

case spokenAudio

## See Also

### Microphone injection modes

`case none`

A mode that indicates not to use spoken audio injection.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/microphoneinjectionmode/none

- AVFAudio
- AVAudioSession
- AVAudioSession.MicrophoneInjectionMode
- AVAudioSession.MicrophoneInjectionMode.none

Case

# AVAudioSession.MicrophoneInjectionMode.none

A mode that indicates not to use spoken audio injection.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

case none

## Discussion

This is the default mode.

## See Also

### Microphone injection modes

`case spokenAudio`

A mode that indicates to inject spoken audio, like synthesized speech, along with microphone audio.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionmicrophoneinjectionisavailablekey

- AVFAudio
- AVAudioSessionMicrophoneInjectionIsAvailableKey

Global Variable

# AVAudioSessionMicrophoneInjectionIsAvailableKey

A key to retrieve a Boolean value that indicates whether microphone injection is available.

let AVAudioSessionMicrophoneInjectionIsAvailableKey: String

## Discussion

The associated value is an `NSNumber` that represents a Boolean value.

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/servicedisabled)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/undetermined)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/requestrecordpermission(completionhandler:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/granted)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudioapplication/microphoneinjectionpermission-swift.enum/denied),

,#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setpreferredmicrophoneinjectionmode(_:))

)#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/microphoneinjectionmode/spokenaudio);

;#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/microphoneinjectionmode/none).

.#app-main)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionmicrophoneinjectionisavailablekey)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/category-swift.struct/playback

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
- playback

Type Property

# playback

The category for playing recorded music or other sounds that are central to the successful use of your app.

static let playback: AVAudioSession.Category

## Discussion

When using this category, your app audio continues with the Silent switch set to silent or when the screen locks. (The switch is called the _Ring/Silent switch_ on iPhone.) To continue playing audio when your app transitions to the background (for example, when the screen locks), add the `audio` value to the UIBackgroundModes key in your information property list file.

By default, using this category implies that your app’s audio is nonmixable—activating your session will interrupt any other audio sessions which are also nonmixable. To allow mixing for this category, use the `mixWithOthers` option.

## See Also

### Getting Standard Categories

`static let ambient: AVAudioSession.Category`

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

`static let multiRoute: AVAudioSession.Category`

The category for routing distinct streams of audio data to different output devices at the same time.

`static let playAndRecord: AVAudioSession.Category`

The category for recording (input) and playback (output) of audio, such as for a Voice over Internet Protocol (VoIP) app.

`static let record: AVAudioSession.Category`

The category for recording audio while also silencing playback audio.

`static let soloAmbient: AVAudioSession.Category`

The default audio session category.

`static let audioProcessing: AVAudioSession.Category`

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setactive:error:

- AVFAudio
- AVAudioSession
- setActive:error:

Instance Method

# setActive:error:

Activates or deactivates your app’s audio session.

- (BOOL) setActive:(BOOL) active
error:(NSError * *) outError;

## Parameters

`active`

Use `true` to activate your app’s audio session, or `false` to deactivate it.

`outError`

On input, a pointer to an error object. If an error occurs, the framework sets the pointer to an `NSError` object that describes the error. If you don’t want error information, pass in `nil`.

## Return Value

`true` if the system successfully changed the active state; otherwise `false`.

## Discussion

Your app may activate a session with category `playback` when another app is hosting a call, for example to start a `SharePlay` activity. However, your app isn’t permitted to capture the microphone of the active call.

The session fails to activate if another audio session has higher priority than yours (such as a phone call) and neither audio session allows mixing. Deactivating an audio session with running audio objects stops the objects, makes the session inactive, and returns an `AVAudioSessionErrorCodeIsBusy` error.

When your app deactivates a session, the return value is `false` but the active state changes to deactivate.

## See Also

### Activating the audio configuration

`func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws`

Activates or deactivates your app’s audio session using the specified options.

Activates an audio session asynchronously on watchOS.

`struct AVAudioSessionActivationOptions`

Constants that describe the options to pass when activating the audio session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setactive(_:options:)

#app-main)

- AVFAudio
- AVAudioSession
- setActive(\_:options:)

Instance Method

# setActive(\_:options:)

Activates or deactivates your app’s audio session using the specified options.

func setActive(
_ active: Bool,
options: AVAudioSession.SetActiveOptions = []
) throws

## Parameters

`active`

Specify `true` to activate your app’s audio session, or `false` to deactivate it.

`options`

An integer bit mask containing one or more constants from the `AVAudioSession.SetActiveOptions` enumeration.

## Discussion

Your app may activate a session with category `playback` when another app is hosting a call, for example to start a `SharePlay` activity. However, your app isn’t permitted to capture the microphone of the active call.

The session fails to activate if another audio session has higher priority than yours (such as a phone call) and neither audio session allows mixing. Deactivating an audio session with running audio objects stops the objects, makes the session inactive, and returns an `AVAudioSessionErrorCodeIsBusy` error.

When your app deactivates a session, the return value is `false` but the active state changes to deactivate.

## Topics

### Data Types

`struct SetActiveOptions`

Options that provide additional information about your app’s audio intentions upon session deactivation.

## See Also

### Activating the audio configuration

Activates an audio session asynchronously on watchOS.

`struct AVAudioSessionActivationOptions`

Constants that describe the options to pass when activating the audio session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/sharedinstance()

#app-main)

- AVFAudio
- AVAudioSession
- sharedInstance()

Type Method

# sharedInstance()

Returns the shared audio session instance.

## Return Value

The shared audio session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setcategory(_:mode:policy:options:)

#app-main)

- AVFAudio
- AVAudioSession
- setCategory(\_:mode:policy:options:)

Instance Method

# setCategory(\_:mode:policy:options:)

Sets the session category, mode, route-sharing policy, and options.

func setCategory(
_ category: AVAudioSession.Category,
mode: AVAudioSession.Mode,
policy: AVAudioSession.RouteSharingPolicy,
options: AVAudioSession.CategoryOptions = []
) throws

## Parameters

`category`

The category to apply to the audio session. See `AVAudioSession.Category` for supported category values.

`mode`

The audio session mode to apply to the audio session. For a list of values, see `AVAudioSession.Mode`.

`policy`

The route-sharing policy to apply to the audio session. For a list of values, see `AVAudioSession.RouteSharingPolicy`.

`options`

A mask of additional options for handling audio. For a list of constants, see `AVAudioSession.CategoryOptions`.

## Discussion

You specify options only with a default routing policy. With a long-form route-sharing policy, you can use the `playback` category and the `default`, `moviePlayback`, and `spokenAudio` modes.

## See Also

### Configuring standard audio behaviors

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category, mode, and options.

`func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category with the specified options.

`func setCategory(AVAudioSession.Category) throws`

Sets the audio session’s category.

`func setMode(AVAudioSession.Mode) throws`

Sets the audio session’s mode.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setcategory(_:mode:options:)

#app-main)

- AVFAudio
- AVAudioSession
- setCategory(\_:mode:options:)

Instance Method

# setCategory(\_:mode:options:)

Sets the audio session’s category, mode, and options.

func setCategory(
_ category: AVAudioSession.Category,
mode: AVAudioSession.Mode,
options: AVAudioSession.CategoryOptions = []
) throws

## Parameters

`category`

The category to apply to the audio session. See `AVAudioSession.Category` for supported category values.

`mode`

The audio session mode to apply to the audio session. For a list of values, see `AVAudioSession.Mode`.

`options`

A mask of additional options for handling audio. For a list of constants, see `AVAudioSession.CategoryOptions`.

## Discussion

The audio session’s `category` and `mode` together define how your app uses audio. Typically, you set the category and mode before activating the session. You can also set the category or mode while the session is active, but doing so results in an immediate change.

## See Also

### Configuring standard audio behaviors

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws`

Sets the session category, mode, route-sharing policy, and options.

`func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category with the specified options.

`func setCategory(AVAudioSession.Category) throws`

Sets the audio session’s category.

`func setMode(AVAudioSession.Mode) throws`

Sets the audio session’s mode.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setcategory(_:options:)

#app-main)

- AVFAudio
- AVAudioSession
- setCategory(\_:options:)

Instance Method

# setCategory(\_:options:)

Sets the audio session’s category with the specified options.

func setCategory(
_ category: AVAudioSession.Category,
options: AVAudioSession.CategoryOptions = []
) throws

## Parameters

`category`

The category to apply to the audio session. See `AVAudioSession.Category` for supported category values.

`options`

A mask of additional options for handling audio. For a list of constants, see `AVAudioSession.CategoryOptions`.

## Discussion

The audio session’s category defines how you intend to use audio in your app. Typically, you set the category before activating the session. You can also set the category while the session is active, but doing so results in an immediate route change.

You can tailor the behavior of certain categories by specifying a mask of category options. Specifying an unsupported option for the indicated category results in an error. See `AVAudioSession.CategoryOptions` for category compatibility.

## See Also

### Configuring standard audio behaviors

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws`

Sets the session category, mode, route-sharing policy, and options.

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category, mode, and options.

`func setCategory(AVAudioSession.Category) throws`

Sets the audio session’s category.

`func setMode(AVAudioSession.Mode) throws`

Sets the audio session’s mode.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setcategory(_:)

#app-main)

- AVFAudio
- AVAudioSession
- setCategory(\_:)

Instance Method

# setCategory(\_:)

Sets the audio session’s category.

func setCategory(_ category: AVAudioSession.Category) throws

## Parameters

`category`

The category to apply to the audio session. See `AVAudioSession.Category` for supported category values.

## Discussion

The audio session’s category defines how the app uses audio. Typically, you set the category before activating the session. You can also set the category while the session is active, but this results in an immediate route change.

## See Also

### Configuring standard audio behaviors

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws`

Sets the session category, mode, route-sharing policy, and options.

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category, mode, and options.

`func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category with the specified options.

`func setMode(AVAudioSession.Mode) throws`

Sets the audio session’s mode.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setmode(_:)

#app-main)

- AVFAudio
- AVAudioSession
- setMode(\_:)

Instance Method

# setMode(\_:)

Sets the audio session’s mode.

func setMode(_ mode: AVAudioSession.Mode) throws

## Parameters

`mode`

The audio session mode to apply to the audio session. See `AVAudioSession.Mode` for supported mode values.

## Discussion

The audio session’s category and mode together define how your app uses audio. Typically, you set the category and mode before activating the session. You can also set the category or mode while the session is active, but doing so results in an immediate change.

## See Also

### Configuring standard audio behaviors

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, policy: AVAudioSession.RouteSharingPolicy, options: AVAudioSession.CategoryOptions) throws`

Sets the session category, mode, route-sharing policy, and options.

`func setCategory(AVAudioSession.Category, mode: AVAudioSession.Mode, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category, mode, and options.

`func setCategory(AVAudioSession.Category, options: AVAudioSession.CategoryOptions) throws`

Sets the audio session’s category with the specified options.

`func setCategory(AVAudioSession.Category) throws`

Sets the audio session’s category.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setintendedspatialexperience(_:)

#app-main)

- AVFAudio
- AVAudioSession
- setIntendedSpatialExperience(\_:)

Instance Method

# setIntendedSpatialExperience(\_:)

Sets the spatial audio experience your app intends to provide the user.

@nonobjc
func setIntendedSpatialExperience(_ spatialExperience: any AVAudioSessionSpatialExperience) throws

## Discussion

- spatialExperience: The spatial audio experience to set.

## See Also

### Configuring the spatial experience in visionOS

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/headtrackedspatialexperience

- AVFAudio
- AVAudioSession
- AVAudioSession.HeadTrackedSpatialExperience

Structure

# AVAudioSession.HeadTrackedSpatialExperience

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

struct HeadTrackedSpatialExperience

## Topics

### Instance Properties

`var anchoringStrategy: AVAudioSession.AnchoringStrategy`

`var soundStageSize: AVAudioSession.SoundStageSize`

## Relationships

### Conforms To

- `AVAudioSessionSpatialExperience`
- `Equatable`
- `Sendable`
- `SendableMetatype`

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/fixedspatialexperience

- AVFAudio
- AVAudioSession
- AVAudioSession.FixedSpatialExperience

Structure

# AVAudioSession.FixedSpatialExperience

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

struct FixedSpatialExperience

## Topics

### Instance Properties

`var soundStageSize: AVAudioSession.SoundStageSize`

## Relationships

### Conforms To

- `AVAudioSessionSpatialExperience`
- `Equatable`
- `Sendable`
- `SendableMetatype`

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/bypassedspatialexperience

- AVFAudio
- AVAudioSession
- AVAudioSession.BypassedSpatialExperience

Structure

# AVAudioSession.BypassedSpatialExperience

An experience that bypasses system-provided audio spatialization.

struct BypassedSpatialExperience

## Relationships

### Conforms To

- `AVAudioSessionSpatialExperience`
- `Equatable`
- `Sendable`
- `SendableMetatype`

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/anchoringstrategy

- AVFAudio
- AVAudioSession
- AVAudioSession.AnchoringStrategy

Enumeration

# AVAudioSession.AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

enum AnchoringStrategy

## Topics

### Anchoring strategies

`case automatic`

The system determines the anchoring strategy.

`case front`

The audio session anchors to a person’s concept of front.

`case scene(identifier: String)`

The audio session anchors to a scene.

## Relationships

### Conforms To

- `Equatable`
- `Sendable`
- `SendableMetatype`

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/soundstagesize

- AVFAudio
- AVAudioSession
- AVAudioSession.SoundStageSize

Enumeration

# AVAudioSession.SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

visionOS

enum SoundStageSize

## Topics

### Sound stage sizes

`case automatic`

The system sets the sound stage size.

`case small`

A small sound stage.

`case medium`

A medium sound stage.

`case large`

A large sound stage.

### Initializers

`init?(rawValue: Int)`

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `Hashable`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/isnowplayingcandidate

- AVFAudio
- AVAudioSession
- isNowPlayingCandidate

Instance Property

# isNowPlayingCandidate

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

var isNowPlayingCandidate: Bool { get }

## Discussion

Only a single audio session for an app can be a Now Playing candidate. Designating multiple audio sessions for the same app as Now Playing candidates results in none of them being eligible.

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`func setIsNowPlayingCandidate(Bool) throws`

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/setisnowplayingcandidate(_:)

#app-main)

- AVFAudio
- AVAudioSession
- setIsNowPlayingCandidate(\_:)

Instance Method

# setIsNowPlayingCandidate(\_:)

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

func setIsNowPlayingCandidate(_ inValue: Bool) throws

## Parameters

`inValue`

The new state to set.

## Discussion

Only a single audio session for an app can be a Now Playing candidate. Designating multiple audio sessions for the same app as Now Playing candidates results in none of them being eligible.

## See Also

### Configuring the spatial experience in visionOS

`func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws`

Sets the spatial audio experience your app intends to provide the user.

`protocol AVAudioSessionSpatialExperience`

A protocol that defines types of spatial audio experiences that the system supports.

`struct HeadTrackedSpatialExperience`

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

`struct FixedSpatialExperience`

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

`struct BypassedSpatialExperience`

An experience that bypasses system-provided audio spatialization.

`enum AnchoringStrategy`

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

`enum SoundStageSize`

Constants that specify the perceived size of sounds the audio session plays.

`var isNowPlayingCandidate: Bool`

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/activate(options:completionhandler:)

#app-main)

- AVFAudio
- AVAudioSession
- activate(options:completionHandler:)

Instance Method

# activate(options:completionHandler:)

Activates an audio session asynchronously on watchOS.

func activate(
options: AVAudioSessionActivationOptions = [],

)

## Parameters

`options`

The options to apply when activating the session.

`handler`

The callback the system invokes when the operation completes.

## Discussion

Use this method to play long-form audio—such as music, podcasts, or audio books—on Apple Watch. Before calling this method to activate longform playback, you must call `setCategory(_:mode:policy:options:)`, set the category to `playback`, and route sharing policy to `longForm`.

This method asynchronously activates the audio session. The system calls the completion handler as soon as the session has successfully activated or if the activation fails.

Playback of long-form audio on watchOS requires a Bluetooth audio route. If necessary, the system presents an audio route picker to the user, letting them choose the Bluetooth route. If the user has previously selected a Bluetooth route or if AirPods or other W1-equipped Bluetooth headphones are nearby, the system automatically picks the audio route without displaying a picker view to the user. If no applicable Bluetooth route is selected (either automatically or by the user), the system passes an error to the completion handler.

## See Also

### Activating the audio configuration

`func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws`

Activates or deactivates your app’s audio session using the specified options.

`struct AVAudioSessionActivationOptions`

Constants that describe the options to pass when activating the audio session.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosessionactivationoptions

- AVFAudio
- AVAudioSessionActivationOptions

Structure

# AVAudioSessionActivationOptions

Constants that describe the options to pass when activating the audio session.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

struct AVAudioSessionActivationOptions

## Topics

### Getting Standard Activation Options

`init(rawValue: UInt)`

Creates a new instance with the raw value you specify.

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `ExpressibleByArrayLiteral`
- `OptionSet`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`
- `SetAlgebra`

## See Also

### Activating the audio configuration

`func setActive(Bool, options: AVAudioSession.SetActiveOptions) throws`

Activates or deactivates your app’s audio session using the specified options.

Activates an audio session asynchronously on watchOS.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions

Structure

# AVAudioSession.CategoryOptions

Constants that specify optional audio behaviors.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

struct CategoryOptions

## Overview

Each option is valid only for specific audio session categories.

## Topics

### Creating a Category Option

`init(rawValue: UInt)`

Creates a new instance with the raw value you specify.

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

### Type Properties

`static var allowBluetoothHFP: AVAudioSession.CategoryOptions`

Allows an application to change the default behavior of some audio session categories with regard to whether Bluetooth Hands-Free Profile (HFP) devices are available for routing. The exact behavior depends on the category.

`static var bluetoothHighQualityRecording: AVAudioSession.CategoryOptions`

When this option is specified with a category that supports both input and output, the session will enable full-bandwidth audio in both input & output directions, if the Bluetooth route supports it (e.g. certain AirPods models). It is currently compatible only with mode `default`.

Beta

## Relationships

### Conforms To

- `BitwiseCopyable`
- `Equatable`
- `ExpressibleByArrayLiteral`
- `OptionSet`
- `RawRepresentable`
- `Sendable`
- `SendableMetatype`
- `SetAlgebra`

## See Also

### Inspecting the category configuration

`var category: AVAudioSession.Category`

The current audio session category.

[`var availableCategories: [AVAudioSession.Category]`](https://developer.apple.com/documentation/avfaudio/avaudiosession/availablecategories)

The audio session categories available on the current device.

`struct Category`

Audio session category identifiers.

`var categoryOptions: AVAudioSession.CategoryOptions`

The set of options associated with the current audio session category.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/category-swift.struct/playandrecord

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
- playAndRecord

Type Property

# playAndRecord

The category for recording (input) and playback (output) of audio, such as for a Voice over Internet Protocol (VoIP) app.

static let playAndRecord: AVAudioSession.Category

## Discussion

Your audio continues with the Silent switch set to silent and with the screen locked. (The switch is called the _Ring/Silent switch_ on iPhone.) To continue playing audio when your app transitions to the background (for example, when the screen locks), add the `audio` value to the UIBackgroundModes key in your information property list file.

This category is appropriate for simultaneous recording and playback, and also for apps that record and play back, but not simultaneously.

By default, using this category implies that your app’s audio is nonmixable—activating your session will interrupt any other audio sessions which are also nonmixable. To allow mixing for this category, use the `mixWithOthers` option.

The user must grant permission for audio recording.

This category supports the mirrored version of Airplay. However, AirPlay mirroring will be disabled if the `AVAudioSessionModeVoiceChat` mode is used with this category.

## See Also

### Getting Standard Categories

`static let ambient: AVAudioSession.Category`

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

`static let multiRoute: AVAudioSession.Category`

The category for routing distinct streams of audio data to different output devices at the same time.

`static let playback: AVAudioSession.Category`

The category for playing recorded music or other sounds that are central to the successful use of your app.

`static let record: AVAudioSession.Category`

The category for recording audio while also silencing playback audio.

`static let soloAmbient: AVAudioSession.Category`

The default audio session category.

`static let audioProcessing: AVAudioSession.Category`

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/mixwithothers

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- mixWithOthers

Type Property

# mixWithOthers

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

static var mixWithOthers: AVAudioSession.CategoryOptions { get }

## Discussion

You can set this option explicitly only if the audio session category is `playAndRecord`, `playback`, or `multiRoute`. If you set the audio session category to `ambient`, the session automatically sets this option. Likewise, setting the `duckOthers` or `interruptSpokenAudioAndMixWithOthers` options also enables this option.

Clearing this option and then activating your session interrupts other audio sessions. If you set this option, your app mixes its audio with audio playing in background apps, such as the Music app.

## See Also

### Getting Standard Session Options

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/duckothers

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- duckOthers

Type Property

# duckOthers

An option that reduces the volume of other audio sessions while audio from this session plays.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

static var duckOthers: AVAudioSession.CategoryOptions { get }

## Discussion

You can set this option only if the audio session category is `playAndRecord`, `playback`, or `multiRoute`. Setting it implicitly sets the `mixWithOthers` option.

Use this option to mix your app’s audio with that of others. While your app plays audio, the system reduces the volume of other audio sessions to make yours more prominent. If your app provides occasional spoken audio, such as in a turn-by-turn navigation app or an exercise app, you should also set the `interruptSpokenAudioAndMixWithOthers` option.

Ducking begins when you activate your app’s audio session and ends when you deactivate the session. If you clear this option, activating your session interrupts other audio sessions.

## See Also

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/interruptspokenaudioandmixwithothers

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- interruptSpokenAudioAndMixWithOthers

Type Property

# interruptSpokenAudioAndMixWithOthers

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions { get }

## Discussion

You can set this option only if the audio session category is `playAndRecord`, `playback`, or `multiRoute`. Setting this option also sets `mixWithOthers`.

If you clear this option, audio from your audio session interrupts other sessions. If you set this option, the system mixes your audio with other audio sessions, but interrupts (and stops) audio sessions that use the `spokenAudio` audio session mode. It pauses the audio from other apps as long as your session is active. After your audio session deactivates, the system resumes the interrupted app’s audio.

Set this option if your app’s audio is occasional and spoken, such as in a turn-by-turn navigation app or an exercise app. This avoids intelligibility problems when two spoken audio apps mix. If you set this option, also set the `duckOthers` option unless you have a specific reason not to. Ducking other audio, rather than interrupting it, is appropriate when the other audio isn’t spoken audio.

When you configure your audio session category using this option, notify other apps on the system when you deactivate your session so that they can resume audio playback. To do so, deactivate your session using the `notifyOthersOnDeactivation` option.

do {
try session.setActive(false, options: .notifyOthersOnDeactivation)
} catch let error as NSError {
print("Failed to deactivate audio session: \(error.localizedDescription)")
}

## See Also

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/allowbluetooth



---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/allowbluetootha2dp

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- allowBluetoothA2DP

Type Property

# allowBluetoothA2DP

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

static var allowBluetoothA2DP: AVAudioSession.CategoryOptions { get }

## Discussion

A2DP is a stereo, output-only profile intended for higher bandwidth audio use cases, such as music playback. The system automatically routes to A2DP ports if you configure an app’s audio session to use the `ambient`, `soloAmbient`, or `playback` categories.

Starting with iOS 10.0, apps using the `playAndRecord` category may also allow routing output to paired Bluetooth A2DP devices. To enable this behavior, pass this category option when setting your audio session’s category.

Audio sessions using the `multiRoute` or `record` categories implicitly clear this option. If you clear it, paired Bluetooth A2DP devices don’t show up as available audio output routes.

## See Also

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/allowairplay

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- allowAirPlay

Type Property

# allowAirPlay

An option that determines whether you can stream audio from this session to AirPlay devices.

static var allowAirPlay: AVAudioSession.CategoryOptions { get }

## Discussion

Setting this option enables the audio session to route audio output to AirPlay devices. You can only explicitly set this option if the audio session’s category is set to `playAndRecord`. For most other audio session categories, the system sets this option implicitly.

Audio sessions using the `multiRoute` or `record` categories implicitly clear this option.

## See Also

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var defaultToSpeaker: AVAudioSession.CategoryOptions`

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct/defaulttospeaker

- AVFAudio
- AVAudioSession
- AVAudioSession.CategoryOptions
- defaultToSpeaker

Type Property

# defaultToSpeaker

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

iOSiPadOSMac CatalystvisionOS

static var defaultToSpeaker: AVAudioSession.CategoryOptions { get }

## Discussion

You can set this option only when using the `playAndRecord` category. Use it to modify the category’s routing behavior so audio is always routed to the speaker rather than the receiver, even when other accessories, such as headphones and wireless Bluetooth headphones, are in use.

When using this option, the system doesn’t honor user gestures. For example, plugging in a headset doesn’t cause the route to change to headset mic and headphones, the route remains to the built-in mic and speaker when you’ve set this override.

In the case of using a USB input-only accessory, audio input comes from the accessory, and the system routes audio to the headphones, if attached, or to the speaker if the headphones aren’t plugged in. The use case is to route audio to the speaker instead of the receiver in cases where the audio normally goes to the receiver.

## See Also

### Getting Standard Session Options

`static var mixWithOthers: AVAudioSession.CategoryOptions`

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

`static var duckOthers: AVAudioSession.CategoryOptions`

An option that reduces the volume of other audio sessions while audio from this session plays.

`static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions`

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

`static var allowBluetooth: AVAudioSession.CategoryOptions`

An option that determines whether Bluetooth hands-free devices appear as available input routes.

Deprecated

`static var allowBluetoothA2DP: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

`static var allowAirPlay: AVAudioSession.CategoryOptions`

An option that determines whether you can stream audio from this session to AirPlay devices.

`static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions`

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

---

# https://developer.apple.com/documentation/avfaudio/avaudiosession/categoryoptions-swift.struct)

# The page you're looking for can't be found.

Search developer.apple.comSearch Icon

---

