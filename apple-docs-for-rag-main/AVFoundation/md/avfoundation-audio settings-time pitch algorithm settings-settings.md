

- AVFoundation
- Audio settings
-  Time Pitch Algorithm Settings 

API Collection

# Time Pitch Algorithm Settings

The constants that define the values for the time pitch algorithms.

## Overview

In iOS and macOS, the default algorithm for playback for apps linked on or after iOS 15 or macOS 12 is timeDomain.

For iOS versions prior to iOS 15, the default value is lowQualityZeroLatency, and for macOS versions prior to macOS 12, the default value is spectral.

The default value for export and other offline processing is spectral.

For scaled audio edits, such as when the timeMapping of an AVAssetTrackSegment is between `timeRanges` of unequal duration, it’s important to choose an algorithm that supports the full range of edit rates present in the source media. The pitch algorithm spectral is often the best choice due to the highly inclusive range of rates it supports, assuming that it’s desirable to maintain a constant pitch regardless of the edit rate. If it’s desirable to allow the pitch to vary with the edit rate, varispeed is the best choice.

## Topics

### Constants

static let timeDomain: AVAudioTimePitchAlgorithm

A modest quality time pitch algorithm that’s suitable for voice.

static let varispeed: AVAudioTimePitchAlgorithm

A high-quality time pitch algorithm that doesn’t perform pitch correction.

static let spectral: AVAudioTimePitchAlgorithm

A highest-quality time pitch algorithm that’s suitable for music.

static let lowQualityZeroLatency: AVAudioTimePitchAlgorithm

A low-quality and very low computationally intensive pitch algorithm.

Deprecated

## See Also

### Settings

Sample Rate Conversion Settings

The constants that define sample rate converter audio quality settings.

enum AVAudioQuality

The values that specify the sample rate audio quality for encoding and conversion.

Encoder Settings

The constants that define the audio encoder settings for the audio recorder class.

