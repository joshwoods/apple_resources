

- Media Setup
- MSServiceAccount
-  clientSecret 

Instance Property

# clientSecret

A string that authenticates the user’s setup request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var clientSecret: String? { get set }
```

## Discussion

The Media Setup framework uses the `clientSecret` to create a token request. Hashed passwords are acceptable, but plaintext passwords are not.

## See Also

### Providing Parameters for an OAuth Request

var authorizationTokenURL: URL?

A URL the system can access to request an OAuth token for the user’s HomePod speakers.

var authorizationScope: String?

A list of permissions for the token request.

var clientID: String?

A user identifier for the token request.

var configurationURL: URL?

The path to access the configuration endpoint of your streaming media service for HomePod.

