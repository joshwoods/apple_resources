

- Authentication Services
- ASAuthorizationAppleIDCredential
-  fullName 

Instance Property

# fullName

The user’s full name from their Apple ID or a user-submitted value provided from the Sign in with Apple UI.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var fullName: PersonNameComponents? { get }
```

## Discussion

Apple doesn’t receive the user’s full name shared with the system UI. The raw data is passed directly to your app from the browser and is not included in the user’s identity token. For more information, visit Authenticating users with Sign in with Apple.

Tip

To help prevent cross-site scripting attacks, validate and sanitize the user-submitted first and last name values before storing on your app servers.

## See Also

### Getting Contact Information

var authorizedScopes: [ASAuthorization.Scope]

The contact information the user authorized your app to access.

var email: String?

The user’s email address.

