

- CarPlay
-  CPNowPlayingModeSports 

Class

# CPNowPlayingModeSports

The sports mode represents a layout for now playing suited to live-streaming or recorded playback of a sporting event that features exactly two teams.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
class CPNowPlayingModeSports
```

## Topics

### Initializers

init(leftTeam: CPNowPlayingSportsTeam, rightTeam: CPNowPlayingSportsTeam, eventStatus: CPNowPlayingSportsEventStatus?, backgroundArtwork: UIImage?)

Initialize a sports mode for display on the CarPlay now playing screen.

### Instance Properties

var backgroundArtwork: UIImage?

A large colorful image for the background of the now playing screen. A gradient or crossfade image works best, especially when it includes the primary colors of each team. Provide an image no larger than 500x500.

var eventStatus: CPNowPlayingSportsEventStatus?

A representation of the current event status. See

var leftTeam: CPNowPlayingSportsTeam

The sports team that should appear on the left side of the now playing screen. This is commonly (but not always) the AWAY or VISITING team. This team will be on the left in all layouts; it does not flip to the right side when in a right-to-left language or a right-hand-drive vehicle.

var rightTeam: CPNowPlayingSportsTeam

The sports team that should appear on the right side of the now playing screen. This is commonly (but not always) the HOME team. This team will be on the right in all layouts; it does not flip to the left side when in a right-to-left language or a right-hand-drive vehicle.

## Relationships

### Inherits From

- CPNowPlayingMode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

