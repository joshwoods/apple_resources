

- GameKit
- GKLocalPlayer
-  isUnderage 

Instance Property

# isUnderage

A Boolean value that indicates whether the local player is underage.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var isUnderage: Bool { get }
```

## Mentioned in 

Authenticating a player

## Discussion

If this property is true, Game Center disables some features for the local player. On all platforms, Game Center provides the value for the underage property for the Game Center account that the player signs into on the device. Note that the Game Center account defaults to the iCloud account that the player signs into on the device, but the player can sign into a different Game Center account.

## See Also

### Determining Whether the Player Is Underage or Restricted

var isMultiplayerGamingRestricted: Bool

A Boolean value that indicates whether the player can join multiplayer games.

var isPersonalizedCommunicationRestricted: Bool

A Boolean value that indicates whether the player can use personalized communication on the device.

