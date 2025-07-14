

- Authentication Services
- ASAuthorizationAppleIDProvider
- ASAuthorizationAppleIDProvider.CredentialState
-  ASAuthorizationAppleIDProvider.CredentialState.authorized 

Case

# ASAuthorizationAppleIDProvider.CredentialState.authorized

The user is authorized.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case authorized
```

## See Also

### User Credential States

case notFound

The user hasn’t established a relationship with Sign in with Apple.

case revoked

The given user’s authorization has been revoked and they should be signed out.

case transferred

The app has been transferred to a different team, and you need to migrate the user’s identifier.

