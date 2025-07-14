

- CarPlay
-  CPNowPlayingSportsTeam 

Class

# CPNowPlayingSportsTeam

A representation of a sports team for the now playing screen, in sports that have exactly two teams.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
class CPNowPlayingSportsTeam
```

## Topics

### Initializers

init(name: String, logo: CPNowPlayingSportsTeamLogo, teamStandings: String?, eventScore: String, possessionIndicator: UIImage?, favorite: Bool)

Initialize a sports team for display on the now playing screen.

### Instance Properties

var eventScore: String

The numeric score string for this team in the current event. Depending on the size of the car screen, a maximum of 3 to 5 characters may be displayed.

var isFavorite: Bool

If true, the team is marked with a star to indicate it has been saved as a user favorite.

var logo: CPNowPlayingSportsTeamLogo

The team logo or, if no logo is available, the initials/abbreviation for this team. See @c CPNowPlayingSportsTeamLogo.

var name: String

A localized, user-visible name for this sports team.

var possessionIndicator: UIImage?

An optional indicator used to indicate possession by this team. Only one team should have possession at a given time.

var teamStandings: String?

An optional additional label displayed near the team name. This could be a win-loss ratio string, team standings, or other statistics relevant to this team. Depending on the size of the car screen, a maximum of 15-20 characters may be displayed.

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

