

- AVFAudio
- AVAudioSession
-  AVAudioSession.CategoryOptions 

Structure

# AVAudioSession.CategoryOptions

Constants that specify optional audio behaviors.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct CategoryOptions
```

## Overview

Each option is valid only for specific audio session categories.

## Topics

### Creating a Category Option

init(rawValue: UInt)

Creates a new instance with the raw value you specify.

### Getting Standard Session Options

static var mixWithOthers: AVAudioSession.CategoryOptions

An option that indicates whether audio from this session mixes with audio from active sessions in other audio apps.

static var duckOthers: AVAudioSession.CategoryOptions

An option that reduces the volume of other audio sessions while audio from this session plays.

static var interruptSpokenAudioAndMixWithOthers: AVAudioSession.CategoryOptions

An option that determines whether to pause spoken audio content from other sessions when your app plays its audio.

static var allowBluetooth: AVAudioSession.CategoryOptions

An option that determines whether Bluetooth hands-free devices appear as available input routes.

static var allowBluetoothA2DP: AVAudioSession.CategoryOptions

An option that determines whether you can stream audio from this session to Bluetooth devices that support the Advanced Audio Distribution Profile (A2DP).

static var allowAirPlay: AVAudioSession.CategoryOptions

An option that determines whether you can stream audio from this session to AirPlay devices.

static var defaultToSpeaker: AVAudioSession.CategoryOptions

An option that determines whether audio from the session defaults to the built-in speaker instead of the receiver.

static var overrideMutedMicrophoneInterruption: AVAudioSession.CategoryOptions

An option that indicates whether the system interrupts the audio session when it mutes the built-in microphone.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Inspecting the category configuration

var category: AVAudioSession.Category

The current audio session category.

var availableCategories: [AVAudioSession.Category]

The audio session categories available on the current device.

struct Category

Audio session category identifiers.

var categoryOptions: AVAudioSession.CategoryOptions

The set of options associated with the current audio session category.

