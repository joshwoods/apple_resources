

- AVFoundation
- AVPlayer
-  AVPlayer.HDRMode 

Structure

# AVPlayer.HDRMode

A bitfield type that specifies an HDR mode.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+tvOS 11.2–18.4DeprecatedvisionOS 1.0+

``` source
struct HDRMode
```

## Overview

These modes define the available HDR modes. Query availableHDRModes to find the HDR modes available for a device.

## Topics

### HDR Modes

static var hlg: AVPlayer.HDRMode

The Hybrid Log-Gamma HDR mode is available.

static var hdr10: AVPlayer.HDRMode

The HDR10 HDR mode is available.

static var dolbyVision: AVPlayer.HDRMode

The Dolby Vision HDR mode is available.

### Initializers

init(rawValue: Int)

Creates an HDR mode with a string value.

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

### Determining HDR Playback Eligibility

class var eligibleForHDRPlayback: Bool

A Boolean value that indicates whether the current device can present content to an HDR display.

class var availableHDRModes: AVPlayer.HDRMode

The HDR modes that are available for playback.

class let eligibleForHDRPlaybackDidChangeNotification: NSNotification.Name

A notification that’s posted whenever HDR playback eligibility changes.

