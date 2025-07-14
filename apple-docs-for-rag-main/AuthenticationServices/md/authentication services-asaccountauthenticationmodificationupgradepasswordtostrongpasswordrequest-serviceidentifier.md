

- Authentication Services
- ASAccountAuthenticationModificationUpgradePasswordToStrongPasswordRequest
-  serviceIdentifier 

Instance Property

# serviceIdentifier

An identifier that represents a particular service that the user needs a credential for, like a web site.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var serviceIdentifier: ASCredentialServiceIdentifier { get }
```

## See Also

### Creating Upgrade Requests in Your App

init(user: String, serviceIdentifier: ASCredentialServiceIdentifier, userInfo: [AnyHashable : Any]?)

Creates a request to upgrade from using a weak password to using a strong system-generated password.

var user: String

The user name of the account to upgrade.

var userInfo: [AnyHashable : Any]?

A dictionary that contains values to pass to your account modification extension.

