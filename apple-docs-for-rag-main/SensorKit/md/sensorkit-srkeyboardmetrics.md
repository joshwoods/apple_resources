

- SensorKit
-  SRKeyboardMetrics 

Class

# SRKeyboardMetrics

The configuration of a device’s keyboard and its usage patterns.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRKeyboardMetrics
```

## Overview

The keyboardMetrics sensor provides this class as its sample type.

## Topics

### Inspecting Keyboard Configuration and Sessions

var duration: TimeInterval

The duration that the report spans.

var keyboardIdentifier: String

The identifier of the keyboard in the keyboard list.

var version: String

The version of keyboard metrics.

var width: Measurement&lt;UnitLength>

The width, in millimeters, of the keyboard in the report.

var height: Measurement&lt;UnitLength>

The height, in millimeters, of the keyboard in the report.

var inputModes: [String]

The active keyboard languages in the session.

var sessionIdentifiers: [String]

The identifiers for the keyboard sessions that report metrics to the sample.

### Quantifying Key Use

var totalWords: Int

The total number of typed words for the keyboard.

var totalAlteredWords: Int

The total number of altered words for the keyboard.

var totalTaps: Int

The total number of taps for the keyboard.

var totalDrags: Int

The total number of drags for the keyboard.

var totalDeletes: Int

The total number of deletions for the keyboard.

var totalEmojis: Int

The total number of emojis for the keyboard.

var totalPaths: Int

The total number of completed paths for the keyboard.

var totalPathTime: TimeInterval

The total time to complete paths for the keyboard.

var totalPathLength: Measurement&lt;UnitLength>

The total length of completed paths for the keyboard.

var totalAutoCorrections: Int

The total number of autocorrections for the keyboard.

var totalSpaceCorrections: Int

The total number of space corrections for the keyboard.

var totalRetroCorrections: Int

The total number of retro corrections for the keyboard.

var totalTranspositionCorrections: Int

The total number of transposition corrections for the keyboard.

var totalInsertKeyCorrections: Int

The total number of Insert key corrections for the keyboard.

var totalSkipTouchCorrections: Int

The total number of skip touch corrections for the keyboard.

var totalNearKeyCorrections: Int

The total number of near key corrections for the keyboard.

var totalSubstitutionCorrections: Int

The total number of substitution corrections for the keyboard.

var totalHitTestCorrections: Int

The total number of hit test corrections for the keyboard.

var totalTypingDuration: TimeInterval

The total amount of typing time for the keyboard.

var totalPathPauses: Int

The total number of pauses while drawing a path for a word.

var totalPauses: Int

The total number of pauses during the session.

var totalTypingEpisodes: Int

The total number of continuous typing episodes during the session.

### Timing Key Use

class ProbabilityMetric

A likelihood of occurrence.

var touchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down to touch up for any key.

var touchUpDown: ProbabilityMetric&lt;UnitDuration>

The duration between touch up and touch down for any key.

var spaceTouchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch up of all Space bar events for the keyboard.

var deleteTouchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch up of all Delete key events for the keyboard.

var shortWordCharKeyTouchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch up of all character keys in short words for the keyboard.

var touchDownDown: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch down for any key.

var charKeyToPrediction: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a character key and touch down on a word in the prediction bar.

var shortWordCharKeyToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a character key and touch down on any sequential character key in a short word.

var charKeyToAnyTapKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a character key and touch down on the next sequential key.

var anyTapToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of any key and touch down on a sequential character key.

var spaceToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential character key.

var charKeyToSpaceKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a character key and touch down of a sequential Space bar.

var spaceToDeleteKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential Delete key.

var deleteToSpaceKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential Space bar.

var spaceToSpaceKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential Space bar.

var spaceToShiftKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential Shift key.

var spaceToPlaneChangeKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential plane change key.

var spaceToPredictionKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential selection from the prediction bar.

var deleteToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential character key.

var charKeyToDelete: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a character key and touch down of a sequential Delete key.

var deleteToDelete: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential Delete key.

var deleteToDeletes: [ProbabilityMetric&lt;UnitDuration>]

The duration between touch up of the Delete key and touch down of a sequential Delete key for an entire word.

var deleteToShiftKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential Shift key.

var deleteToPlaneChangeKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential plane change key.

var anyTapToPlaneChangeKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of any key and touch down on a plane change key.

var planeChangeToAnyTap: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a plane change key and touch down on the next sequential key.

var charKeyToPlaneChangeKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a character key and touch down of a sequential plane change key.

var planeChangeKeyToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a plane change key and touch down of any key.

var deleteToPath: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential path.

var pathToDelete: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a continuous path.

var spaceToPath: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down to begin a sequential path.

var pathToSpace: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a path and touch down of a sequential Space bar.

var pathToPath: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a path and touch down of a sequential path.

var longWordTouchDownUp: [ProbabilityMetric&lt;UnitDuration>]

The duration between touch down and touch up of the character keys of all the long words in the session.

var longWordTouchDownDown: [ProbabilityMetric&lt;UnitDuration>]

The duration between touch down and touch down of the character keys of all the long words in the session.

var longWordTouchUpDown: [ProbabilityMetric&lt;UnitDuration>]

The duration between touch up and touch down of the character keys of all the long words in the session.

var pathTypingSpeed: Double

The QuickType words per minute in the session.

var typingSpeed: Double

The user’s typing rate in characters per second.

### Measuring Key Use

var longWordUpErrorDistance: [ProbabilityMetric&lt;UnitLength>]

The distance from the touch up to the center of the intended key of the characters of a long word.

var longWordDownErrorDistance: [ProbabilityMetric&lt;UnitLength>]

The distance from the touch down to the center of the intended key of the characters of a long word.

var upErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the center of any key.

var downErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the center of any key.

var spaceUpErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the right centroid of the Space bar.

var spaceDownErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the right centroid of the Space bar.

var deleteUpErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the center of the Delete key.

var deleteDownErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the center of the Delete key.

var shortWordCharKeyUpErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the center of the intended key of a character in a short word.

var shortWordCharKeyDownErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the center of the intended key of a character in a short word.

var pathErrorDistanceRatio: [NSNumber]

Sample values of the ratio of error distance between the intended and actual path.

### Inferring Sentiment

func wordCount(for: SRKeyboardMetrics.SentimentCategory) -> Int

Provides the number of typed words for the specified sentiment in the report.

func emojiCount(for: SRKeyboardMetrics.SentimentCategory) -> Int

Provides the number of typed emojis for the specified sentiment in the report.

enum SentimentCategory

Moods that the framework determines by analyzing the user’s input.

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

### Interpreting data

class SRAmbientLightSample

The amount of ambient light in the user’s environment.

class SRDeviceUsageReport

The frequency and relative duration that the user uses their device, particular Apple apps, or websites.

class SRMediaEvent

A user interaction with a media object, such as an image or a video.

class SRMessagesUsageReport

An object that describes the user’s Messages app activity over a period of time.

class SRPhoneUsageReport

An object that describes the user’s phone activity over a period of time.

class SRVisit

The user’s progress in their daily travel routine.

class SRWristDetection

The configuration of a watch on the wearer’s wrist.

