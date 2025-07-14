

- Authentication Services
- ASAccountAuthenticationModificationViewController
-  changePasswordWithoutUserInteraction(for:existingCredential:newPassword:userInfo:) 

Instance Method

# changePasswordWithoutUserInteraction(for:existingCredential:newPassword:userInfo:)

Upgrades a user’s weak password to a strong password.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
func changePasswordWithoutUserInteraction(
    for serviceIdentifier: ASCredentialServiceIdentifier,
    existingCredential: ASPasswordCredential,
    newPassword: String,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`serviceIdentifier`  

An identifier that represents a particular service that the user needs a credential for, like a web site.

`existingCredential`  

The current password credential for the service.

`newPassword`  

A new, automatically generated, strong password for the service to use.

`userInfo`  

A dictionary that contains app-specific values when the request to upgrade to Sign in with Apple initiates from the parent app. If the request to upgrade to Sign in with Apple doesn’t initiate from the app, this parameter is `nil`.

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Discussion

If the extension’s `Info.plist` file includes the ASAccountAuthenticationModificationPasswordGenerationRequirements key, the value of `newPassword` satisfies the specified requirements.

## See Also

### Upgrading to Strong Passwords

func prepareInterfaceToChangePassword(for: ASCredentialServiceIdentifier, existingCredential: ASPasswordCredential, newPassword: String, userInfo: [AnyHashable : Any]?)

Prepares the view controller’s interface that displays when upgrading from a weak password to a strong password.

ASAccountAuthenticationModificationSupportsStrongPasswordChange

A Boolean value that indicates whether the extension supports upgrading a user’s password to a strong password.

ASAccountAuthenticationModificationPasswordGenerationRequirements

The rules the system satisfies when generating a strong password for your extension during an automatic upgrade.

ASAccountAuthenticationModificationOptOutOfSecurityPromptsOnSignIn

A Boolean value that indicates the system shouldn’t show security recommendation prompts when users sign in using the app.

