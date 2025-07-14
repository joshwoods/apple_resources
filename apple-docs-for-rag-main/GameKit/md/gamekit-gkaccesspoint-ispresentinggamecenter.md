

- GameKit
- GKAccessPoint
-  isPresentingGameCenter 

Instance Property

# isPresentingGameCenter

A Boolean value that indicates whether the game is presenting the Game Center dashboard.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var isPresentingGameCenter: Bool { get }
```

## Mentioned in 

Adding an access point to your game

## Discussion

This property is true when the player taps the access point control and false when the player dismisses the Game Center dashboard. This is an observable property.

## See Also

### Displaying the access point

var isActive: Bool

A Boolean value that determines whether to display the access point.

var isVisible: Bool

A Boolean value that indicates whether the access point is visible.

var showHighlights: Bool

A Boolean value that indicates whether to display highlights for achievements and current ranks for leaderboards.

