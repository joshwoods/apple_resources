

- Media Setup
- MSServiceAccount
-  configurationURL 

Instance Property

# configurationURL

The path to access the configuration endpoint of your streaming media service for HomePod.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var configurationURL: URL? { get set }
```

## See Also

### Providing Parameters for an OAuth Request

var authorizationTokenURL: URL?

A URL the system can access to request an OAuth token for the user’s HomePod speakers.

var authorizationScope: String?

A list of permissions for the token request.

var clientID: String?

A user identifier for the token request.

var clientSecret: String?

A string that authenticates the user’s setup request.

