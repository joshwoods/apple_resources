

- Media Setup
- MSServiceAccount
-  clientID 

Instance Property

# clientID

A user identifier for the token request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var clientID: String? { get set }
```

## Discussion

The Media Setup framework uses the `clientID` to create a token request. You can choose the identifier format, but the identifier must be unique to the current account. You can provide a new identifier each time the user begins HomePod setup.

## See Also

### Providing Parameters for an OAuth Request

var authorizationTokenURL: URL?

A URL the system can access to request an OAuth token for the user’s HomePod speakers.

var authorizationScope: String?

A list of permissions for the token request.

var clientSecret: String?

A string that authenticates the user’s setup request.

var configurationURL: URL?

The path to access the configuration endpoint of your streaming media service for HomePod.

