

- AVKit
-  AVPlaybackSpeed 

Class

# AVPlaybackSpeed

An object that represents a user-selectable playback speed in a playback user interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVPlaybackSpeed
```

## Topics

### Retrieving Default Speeds

class var systemDefaultSpeeds: [AVPlaybackSpeed]

A list of playback speeds the system uses by default.

### Creating a Playback Speed

init(rate: Float, localizedName: String)

Creates a playback speed with a rate and localized name.

### Inspecting Speed Details

var rate: Float

The playback rate to use when you select this speed.

var localizedName: String

A localized name for a speed that’s suitable for display in a user interface.

var localizedNumericName: String

A localized numeric name for a speed that’s suitable for display in a user interface.

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

### Configuring the Playback Speed

var speeds: [AVPlaybackSpeed]

A list of user-selectable playback speeds to show in the playback speed control.

var selectedSpeed: AVPlaybackSpeed?

The currently selected playback speed.

func selectSpeed(AVPlaybackSpeed)

Selects a specified playback speed.

