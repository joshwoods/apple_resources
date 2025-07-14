

- Authentication Services
- ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest
-  user 

Instance Property

# user

The user name of the account to upgrade.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var user: String { get }
```

## See Also

### Creating Upgrade Requests in Your App

init(user: String, serviceIdentifier: ASCredentialServiceIdentifier, userInfo: [AnyHashable : Any]?)

Creates a request to upgrade from using passwords to using Sign in with Apple.

var serviceIdentifier: ASCredentialServiceIdentifier

An identifier that represents a particular service that the user needs a credential for, like a web site.

var userInfo: [AnyHashable : Any]?

A dictionary that contains values to pass to your account modification extension.

