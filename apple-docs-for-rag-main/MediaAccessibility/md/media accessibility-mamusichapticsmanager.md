

- Media Accessibility
-  MAMusicHapticsManager 

Class

# MAMusicHapticsManager

A class that reports information about the Music Haptics feature.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class MAMusicHapticsManager
```

## Overview

Use the shared instance of `MAMusicHapticsManager` to check information about the Music Haptics feature so you can respond accordingly in your app. For example, you can check whether Music Haptics is on, get a notification when it turns on or off, or check whether a haptic track is currently playing along with the Now Playing item.

## Topics

### Getting the shared haptics manager

class var shared: MAMusicHapticsManager

The shared Music Haptics manager object.

### Checking if Music Haptics is on

var isActive: Bool

A Boolean value that indicates whether the system setting for Music Haptics is on.

class let activeStatusDidChangeNotification: NSNotification.Name

A notification that posts when the value of the Music Haptics system setting changes.

### Checking haptic track availability

func checkHapticTrackAvailabilityForMedia(matchingCode: String, completionHandler: ((Bool) -> Void)?)

Checks whether a haptic track is available for the song with the specified International Standard Recording Code (ISRC).

### Observing haptic playback

func addStatusObserver((String, Bool) -> Void) -> (any NSCopying)?

Adds an observer to monitor the status of haptic playback for the Now Playing song.

func removeStatusObserver(any NSCopying)

Removes the observer monitoring the status of haptic playback for the Now Playing song.

### Supporting types

struct MAMusicHaptics

A namespace for Music Haptics symbols.

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

