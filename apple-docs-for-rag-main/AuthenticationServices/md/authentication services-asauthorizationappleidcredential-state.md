

- Authentication Services
- ASAuthorizationAppleIDCredential
-  state 

Instance Property

# state

An arbitrary string that your app provides to the request that generates the credential.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var state: String? { get }
```

## See Also

### Identifying a User

var identityToken: Data?

A JSON Web Token (JWT) that securely communicates information about the user to the app.

var authorizationCode: Data?

A token that the app uses to interact with the server.

var user: String

An identifier for the authenticated user.

