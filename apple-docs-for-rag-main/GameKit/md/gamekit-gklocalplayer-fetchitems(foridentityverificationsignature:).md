

- GameKit
- GKLocalPlayer
-  fetchItems(forIdentityVerificationSignature:) 

Instance Method

# fetchItems(forIdentityVerificationSignature:)

Generates a signature that you can use to authenticate the local player on your own server.

iOS 13.5+iPadOS 13.5+Mac Catalyst 13.5+macOS 10.15.5+tvOS 13.4.8+visionOS 1.0+watchOS 6.5+

``` source
func fetchItems(forIdentityVerificationSignature completionHandler: ((URL?, Data?, Data?, UInt64, (any Error)?) -> Void)? = nil)
```

``` source
func fetchItemsForIdentityVerificationSignature() async throws -> (URL, Data, Data, UInt64)
```

## Parameters 

`completionHandler`  

A block that GameKit calls when the request completes.

The block receives the following parameters:

publicKeyURL  
The URL for the public encryption key.

signature  
The verification signature data that GameKit generates.

salt  
A random `NSString` that GameKit uses to compute the hash and randomize it.

timestamp  
The signature’s creation date and time.

error  
If an error occurs, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

To generate a signature for your authentication server, you perform steps in the game and pass data to the server, which completes the process.

In your game, follow these steps:

1.  Call the fetchItems(forIdentityVerificationSignature:) method.

2.  Send the completion handler `publicKeyURL`, `signature`, `salt`, and `timestamp` parameters to your authentication server.

3.  Share the teamPlayerID and the bundle ID (see CFBundleIdentifier) with the server. For Apple Arcade games, share the gamePlayerID instead of the teamPlayerID.

On the server, perform these steps:

1.  To mitigate replay attacks, make sure the `timestamp` parameter is recent, and to avoid high network overhead, respect the cache expiration headers.

2.  Download the public key using the `publicKeyURL` parameter.

3.  Verify with the appropriate signing authority that Apple signed the public key.

4.  Concatenate the following information into a data buffer in this order: the teamPlayerID (or gamePlayerID for Apple Arcade) property in UTF-8 format, the bundle ID in UTF-8 format, the `timestamp` parameter in big-endian UInt64 format, and the `salt` parameter.

5.  Use the public key to verify the signature of the concatenated data buffer using the RSASSA-PKCS1-v1_5 algorithm.

If the generated and retrieved signatures match, GameKit authenticates the local player.

Important

Trust only the fields in the signed payload. Consider other data, such as nicknames, as player-provided information.

## See Also

### Authenticating the Local Player

var authenticateHandler: ((UIViewController?, (any Error)?) -> Void)?

A handler that GameKit calls while authenticating the local player.

var isAuthenticated: Bool

A Boolean value that indicates whether a local player has signed in to Game Center.

static let GKPlayerAuthenticationDidChangeNotificationName: NSNotification.Name

A notification that posts after GameKit authenticates the local player.

