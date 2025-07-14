

- GameKit
- GKLocalPlayer
-  isMultiplayerGamingRestricted 

Instance Property

# isMultiplayerGamingRestricted

A Boolean value that indicates whether the player can join multiplayer games.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var isMultiplayerGamingRestricted: Bool { get }
```

## Mentioned in 

Authenticating a player

## Discussion

If this property is true, the local player can’t join multiplayer games. If your game uses a custom multiplayer feature, you should disable it.

On iOS and macOS, the value for this property comes from the Screen Time settings that the system syncs between devices using the same iCloud account. To change this value when testing your game, see Restrict Game Center section of Use parental controls on your child’s iPhone, iPad, and iPod touch and Change Content Restrictions settings in Screen Time on Mac.

On tvOS, players set this value on the device using the Restrictions menu. This setting is local only; the system doesn’t sync this setting to other devices. To change this value when testing your game, see Restrict access to content on Apple TV.

## See Also

### Determining Whether the Player Is Underage or Restricted

var isUnderage: Bool

A Boolean value that indicates whether the local player is underage.

var isPersonalizedCommunicationRestricted: Bool

A Boolean value that indicates whether the player can use personalized communication on the device.

