

- GameKit
- GKPlayer
-  anonymousGuestPlayer(withIdentifier:) 

Type Method

# anonymousGuestPlayer(withIdentifier:)

Creates a guest player with the specified identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func anonymousGuestPlayer(withIdentifier guestIdentifier: String) -> Self
```

## Parameters 

`guestIdentifier`  

An identifier to use for the guest player.

## Return Value

A player object that represents the guest.

## Discussion

You can treat a guest player the same as an authenticated player in regard to matchmaking services.

## See Also

### Creating a guest player

var guestIdentifier: String?

A developer-created string that identifies a guest player.

