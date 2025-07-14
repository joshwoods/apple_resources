

- Authentication Services
-  ASAuthorizationAppleIDCredential 

Class

# ASAuthorizationAppleIDCredential

A credential that results from a successful Apple ID authentication.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationAppleIDCredential
```

## Topics

### Identifying a User

var identityToken: Data?

A JSON Web Token (JWT) that securely communicates information about the user to the app.

var authorizationCode: Data?

A token that the app uses to interact with the server.

var state: String?

An arbitrary string that your app provides to the request that generates the credential.

var user: String

An identifier for the authenticated user.

### Getting Contact Information

var authorizedScopes: [ASAuthorization.Scope]

The contact information the user authorized your app to access.

var fullName: PersonNameComponents?

The user’s full name from their Apple ID or a user-submitted value provided from the Sign in with Apple UI.

var email: String?

The user’s email address.

### Detecting User Characteristics

var realUserStatus: ASUserDetectionStatus

A value that indicates whether the user appears to be a real person.

enum ASUserDetectionStatus

Possible values for the real user indicator.

### Instance Properties

var userAgeRange: ASUserAgeRange

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationCredential
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Sign In with Apple

Implementing User Authentication with Sign in with Apple

Provide a way for users of your app to set up an account and start using your services.

Simplifying User Authentication in a tvOS App

Build a fluid sign-in experience for your tvOS apps using AuthenticationServices.

struct SignInWithAppleButton

The view that creates the Sign in with Apple button for display.

Sign in with Apple Entitlement

An entitlement that lets your app use Sign in with Apple.

class ASAuthorizationAppleIDProvider

A mechanism for generating requests to authenticate users based on their Apple ID.

