

- Media Setup
-  MSServiceAccount 

Class

# MSServiceAccount

Account details for accessing a streaming media service.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class MSServiceAccount
```

## Topics

### Presenting Account Information to the User

init(serviceName: String, accountName: String)

Creates a new account.

var serviceName: String

The localized name of the streaming media service.

var accountName: String

The user’s display name, email address, or other identifier in a streaming media service.

### Providing Parameters for an OAuth Request

var authorizationTokenURL: URL?

A URL the system can access to request an OAuth token for the user’s HomePod speakers.

var authorizationScope: String?

A list of permissions for the token request.

var clientID: String?

A user identifier for the token request.

var clientSecret: String?

A string that authenticates the user’s setup request.

var configurationURL: URL?

The path to access the configuration endpoint of your streaming media service for HomePod.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### HomePod Configuration

class MSSetupSession

An object that manages the transfer of configuration information between your app, the system, your media service, and HomePod speakers.

