

- Authentication Services
- ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
- ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle
-  ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle.conditional 

Case

# ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle.conditional

Perform a conditional request. This style of request is meant to opportunistically add passkeys to existing password-based accounts, at the discretion of the user’s credential manager. It should be performed shortly after a user has signed in with a password. If the user is using a password and passkey manager, and certain internal conditions of that credential manager are met (e.g. the user signed in recently with a matching password-based account and does not yet have a passkey for this account), then this request may proceed automatically, without further user interaction. If any of the internal conditions are not met, this request will return an error without showing any UI to the user, and may be retried the next time they sign in.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case conditional
```

