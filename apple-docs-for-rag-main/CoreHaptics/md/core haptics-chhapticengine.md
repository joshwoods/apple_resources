

- Core Haptics
-  CHHapticEngine 

Class

# CHHapticEngine

An object that represents the connection to the haptic server.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
class CHHapticEngine
```

## Mentioned in 

Playing a single-tap haptic pattern

Preparing your app to play haptics

## Overview

If you want your app to play custom haptics, you need to create a haptic engine. The haptic engine establishes the connection between your app and the underlying device hardware. Even though you can define a haptic pattern without an engine, you need the engine to play that pattern.

Even though your app makes a request through the haptic engine, the operating system could still override the request with system services, like haptics from system notifications.

### Prepare Your App To Play Haptics

To prepare your app to play haptics, follow these steps, as demonstrated in the code below:

1.  Create a haptic engine instance. Maintain a strong reference to it so it doesn’t go out of scope while the haptic is playing.

2.  Call the haptic engine’s start(completionHandler:) for an asynchronous start, or start() to start the engine synchronously (immediately).

3.  Stop the engine by calling stop(completionHandler:) when your app finishes haptic playback.

- Swift
- Objective-C

```
```

```
```

Although it’s possible to create content—CHHapticPattern instances—independent of a CHHapticEngine, your app must use an engine to play that content.

## Topics

### Initializing a Haptic Engine

init() throws

Creates an instance of the haptic engine.

init(audioSession: AVAudioSession?) throws

Creates a haptic engine from an audio session.

### Starting and Stopping the Haptic Engine

func start() throws

Synchronously starts the haptic engine.

func start(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously starts the haptic engine.

func stop(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously stops the haptic engine and executes the completion handler once the engine has stopped.

typealias CompletionHandler

A typealias for a completion handler that the engine calls after starting or stopping.

### Creating Haptic Pattern Players

Factory methods for creating player objects for haptic playback.

func makePlayer(with: CHHapticPattern) throws -> any CHHapticPatternPlayer

Creates a standard haptic pattern player from a haptic pattern.

func makeAdvancedPlayer(with: CHHapticPattern) throws -> any CHHapticAdvancedPatternPlayer

Creates an advanced haptic pattern player from a haptic pattern.

### Modifying Playback Properties

var playsAudioOnly: Bool

A Boolean value that indicates whether the engine ignores haptic events and plays audio events only.

var playsHapticsOnly: Bool

A Boolean value that indicates whether the engine ignores audio events.

var isMutedForAudio: Bool

A Boolean value that indicates whether the engine mutes audio.

var isMutedForHaptics: Bool

A Boolean value that indicates whether the engine mutes haptics.

### Playing a Pattern

func playPattern(from: URL) throws

Plays a pattern that’s defined in a file at the specified URL.

func playPattern(from: Data) throws

Plays a pattern from the specified data.

### Registering Audio Resources

func registerAudioResource(URL, options: [AnyHashable : Any]) throws -> CHHapticAudioResourceID

Registers an external audio to use as a custom waveform.

func unregisterAudioResource(CHHapticAudioResourceID) throws

Unregisters an external audio file that you previously registered with the engine.

typealias CHHapticAudioResourceID

A type that identifies a custom audio resource.

### Monitoring Finished Playback

func notifyWhenPlayersFinished(finishedHandler: CHHapticEngine.FinishedHandler)

Notifies you when all haptic pattern players have finished playing their haptic patterns.

typealias FinishedHandler

A type alias for a completion handler to execute after finishing haptic playback.

enum FinishedAction

Possible actions to take after the haptic engine finishes execution.

### Handling Haptic Engine Resets

var resetHandler: CHHapticEngine.ResetHandler

A block that the haptic engine calls after recovering from a haptic server error.

typealias ResetHandler

A typealias for the block that the haptic engine calls after being reset.

### Handling Haptic Engine Stoppages

var stoppedHandler: CHHapticEngine.StoppedHandler

A closure the haptic engine calls when it stops due to external causes.

typealias StoppedHandler

A typealias for the block that the haptic engine calls after it stops due to an external cause.

enum StoppedReason

The enumeration of reasons the haptic engine stopped running.

### Getting the Current Media Time

var currentTime: TimeInterval

The absolute time, in seconds, to use for scheduling haptic and audio events.

var CHHapticTimeImmediate: TimeInterval

A time constant used to schedule a command immediately.

### Querying System Capabilities

class func capabilitiesForHardware() -> any CHHapticDeviceCapability

Returns a device capability object that describes the device’s haptic support and limitations.

protocol CHHapticDeviceCapability

A protocol that defines haptics and audio capabilities of a device.

protocol CHHapticParameterAttributes

A protocol for providing default, mininum, and maximum values of a parameter.

func attributes(forDynamicParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes

Requests the haptic device’s attributes for a dynamic parameter.

**Required**

### Managing Power

var isAutoShutdownEnabled: Bool

A Boolean value that indicates whether the haptic engine starts and stops automatically on request from one of its pattern players, or when idle.

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

## See Also

### Essentials

Preparing your app to play haptics

Set up your app to play haptics.

Playing a single-tap haptic pattern

Create and play a transient haptic pattern from a dictionary literal inline.

class CHHapticPattern

An object representing a haptic waveform.

protocol CHHapticPatternPlayer

A protocol that defines a standard pattern player capable of playing haptic patterns with fixed parameters.

protocol CHHapticAdvancedPatternPlayer

A protocol that defines an advanced pattern player capable of looping, seeking, pausing, and resuming haptic playback.

