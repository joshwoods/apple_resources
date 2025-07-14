

- Authentication Services
- ASAccountAuthenticationModificationReplacePasswordWithSignInWithAppleRequest
-  init(user:serviceIdentifier:userInfo:) 

Initializer

# init(user:serviceIdentifier:userInfo:)

Creates a request to upgrade from using passwords to using Sign in with Apple.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
init(
    user: String,
    serviceIdentifier: ASCredentialServiceIdentifier,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`user`  

The user name of the account to upgrade.

`serviceIdentifier`  

An identifier that represents a particular service that the user needs a credential for, like a web site.

`userInfo`  

A dictionary that contains values to pass to your account modification extension.

## Return Value

An initialized request object with details about the account to upgrade to Sign in with Apple.

## Discussion

If your extension needs information to authenticate with your server, such as an authentication token, set it in the `userInfo` dictionary before calling this method.

## See Also

### Creating Upgrade Requests in Your App

var user: String

The user name of the account to upgrade.

var serviceIdentifier: ASCredentialServiceIdentifier

An identifier that represents a particular service that the user needs a credential for, like a web site.

var userInfo: [AnyHashable : Any]?

A dictionary that contains values to pass to your account modification extension.

