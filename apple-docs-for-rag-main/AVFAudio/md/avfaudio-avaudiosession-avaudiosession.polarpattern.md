

- AVFAudio
- AVAudioSession
-  AVAudioSession.PolarPattern 

Structure

# AVAudioSession.PolarPattern

Constants that describe the possible polar patterns of the data source on an iOS device.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct PolarPattern
```

## Overview

The direction of a polar pattern is relative to the orientation of the data source. For example, you can use the cardioid pattern with a back-facing data source to more clearly record sound from behind the device, or with a front-facing data source to more clearly record sound from in front of the device (such as the user’s voice).

## Topics

### Creating a Polar Pattern

init(rawValue: String)

Creates a new instance with the raw value you specify.

### Getting Standard Polar Patterns

static let stereo: AVAudioSession.PolarPattern

A polar pattern that captures a stereo image of an audio source.

static let cardioid: AVAudioSession.PolarPattern

A data source that’s most sensitive to sound from the direction of the data source and is nearly insensitive to sound from the opposite direction.

static let subcardioid: AVAudioSession.PolarPattern

A data source that’s most sensitive to sound from the direction of the data source and is less sensitive to sound from the opposite direction.

static let omnidirectional: AVAudioSession.PolarPattern

A data source that’s equally sensitive to sound from any direction.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Microphone Directivity

var selectedPolarPattern: AVAudioSession.PolarPattern?

The data source’s active polar pattern.

var supportedPolarPatterns: [AVAudioSession.PolarPattern]?

The set of directivity configurations supported by the data source.

var preferredPolarPattern: AVAudioSession.PolarPattern?

The preferred directivity configuration for the data source.

func setPreferredPolarPattern(AVAudioSession.PolarPattern?) throws

Selects the preferred directivity configuration for the data source.

