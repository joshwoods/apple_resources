

- AVFAudio
- AVAudioSession
-  AVAudioSession.SetActiveOptions 

Structure

# AVAudioSession.SetActiveOptions

Options that provide additional information about your app’s audio intentions upon session deactivation.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct SetActiveOptions
```

## Overview

Use this option to request that the system notify an interrupted app that the interruption has ended and it may resume playback. This option is only valid on session deactivation.

## Topics

### Creating an Activation Option

init(rawValue: UInt)

Creates a new instance with the raw value you specify.

### Getting Standard Options

static var notifyOthersOnDeactivation: AVAudioSession.SetActiveOptions

An option that indicates that the system should notify other apps that you’ve deactivated your app’s audio session.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

