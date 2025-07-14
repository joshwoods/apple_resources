

- Authentication Services
- ASAuthorizationAppleIDCredential
-  authorizedScopes 

Instance Property

# authorizedScopes

The contact information the user authorized your app to access.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var authorizedScopes: [ASAuthorization.Scope] { get }
```

## See Also

### Getting Contact Information

var fullName: PersonNameComponents?

The user’s full name from their Apple ID or a user-submitted value provided from the Sign in with Apple UI.

var email: String?

The user’s email address.

