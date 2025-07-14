

- Authentication Services
- ASAuthorizationAppleIDCredential
-  authorizationCode 

Instance Property

# authorizationCode

A token that the app uses to interact with the server.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var authorizationCode: Data? { get }
```

## Discussion

Your app uses this short-lived token as proof that it has authorization to interact with the server.

The system encodes the object as a string using NSUTF8StringEncoding.

## See Also

### Identifying a User

var identityToken: Data?

A JSON Web Token (JWT) that securely communicates information about the user to the app.

var state: String?

An arbitrary string that your app provides to the request that generates the credential.

var user: String

An identifier for the authenticated user.

