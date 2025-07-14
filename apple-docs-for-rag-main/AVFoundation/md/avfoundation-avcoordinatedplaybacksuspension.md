

- AVFoundation
-  AVCoordinatedPlaybackSuspension 

Class

# AVCoordinatedPlaybackSuspension

An object that represents a temporary suspension of coordinated playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVCoordinatedPlaybackSuspension
```

## Overview

See the playback coordinator’s beginSuspension(for:) method for details about suspending playback.

## Topics

### Inspecting a Suspension

var beginDate: Date

The time the suspension begins.

var reason: AVCoordinatedPlaybackSuspension.Reason

The reason for the suspension.

struct Reason

Constants that identify playback suspension reasons.

### Ending a Suspension

func end()

Ends a suspension.

func end(proposingNewTime: CMTime)

Ends a suspension and proposes a new playback time to the group.

### Initializers

init(String)

Creates a suspension with a string.

init(rawValue: String)

Creates a suspension with a raw string value.

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

### Suspending State Coordination

func beginSuspension(for: AVCoordinatedPlaybackSuspension.Reason) -> AVCoordinatedPlaybackSuspension

Tells the coordinator to stop sending playback commands temporarily when the playback object disconnects from the group activity.

func expectedItemTime(atHostTime: CMTime) -> CMTime

Returns a time in the current item’s timeline that the coordinator expects to play at the specified host time.

