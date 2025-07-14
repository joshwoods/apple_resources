

- GameKit
- GKLocalPlayer
-  isAuthenticated 

Instance Property

# isAuthenticated

A Boolean value that indicates whether a local player has signed in to Game Center.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var isAuthenticated: Bool { get }
```

## Mentioned in 

Authenticating a player

## See Also

### Authenticating the Local Player

var authenticateHandler: ((UIViewController?, (any Error)?) -> Void)?

A handler that GameKit calls while authenticating the local player.

func fetchItems(forIdentityVerificationSignature: ((URL?, Data?, Data?, UInt64, (any Error)?) -> Void)?)

Generates a signature that you can use to authenticate the local player on your own server.

static let GKPlayerAuthenticationDidChangeNotificationName: NSNotification.Name

A notification that posts after GameKit authenticates the local player.

