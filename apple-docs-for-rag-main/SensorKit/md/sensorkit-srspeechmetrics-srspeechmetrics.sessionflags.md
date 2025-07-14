

- SensorKit
- SRSpeechMetrics
-  SRSpeechMetrics.SessionFlags 

Structure

# SRSpeechMetrics.SessionFlags

Possible details about processing an audio stream.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct SessionFlags
```

## Overview

Use these flags to determine whether audio processing went through the system voice processor.

## Topics

### Session flags

static var bypassVoiceProcessing: SRSpeechMetrics.SessionFlags

Audio processing bypasses the system voice processor.

### Creating session flags

init(rawValue: UInt)

Creates and returns a new structure with the specified value.

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

### Getting session information

var sessionIdentifier: String

An identifier for the audio session.

var sessionFlags: SRSpeechMetrics.SessionFlags

Details about the audio processing.

var timeSinceAudioStart: TimeInterval

The number of seconds since the start of the audio stream.

var timestamp: Date

The date and time when the speech occurs.

