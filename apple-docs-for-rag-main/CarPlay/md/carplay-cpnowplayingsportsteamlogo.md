

- CarPlay
-  CPNowPlayingSportsTeamLogo 

Class

# CPNowPlayingSportsTeamLogo

A logo image or, if no image is available, an abbreviation or initialism for this team.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
class CPNowPlayingSportsTeamLogo
```

## Topics

### Initializers

init(teamInitials: String)

If no team logo image is available, initialize a team logo with an abbreviation or initialism for this team.

init(teamLogo: UIImage)

Initialize a team logo with an image representation of this team. Provide an image no larger than 350x350; larger images will be resized down.

### Instance Properties

var initials: String?

An abbreviation or initialism for this team, used only if no logo image is available for this team.

var logo: UIImage?

A team logo image for this team.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

