

- GameKit
- GKPlayer
-  guestIdentifier 

Instance Property

# guestIdentifier

A developer-created string that identifies a guest player.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var guestIdentifier: String? { get }
```

## See Also

### Creating a guest player

class func anonymousGuestPlayer(withIdentifier: String) -> Self

Creates a guest player with the specified identifier.

