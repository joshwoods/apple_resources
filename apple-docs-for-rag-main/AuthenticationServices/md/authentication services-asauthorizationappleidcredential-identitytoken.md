

- Authentication Services
- ASAuthorizationAppleIDCredential
-  identityToken 

Instance Property

# identityToken

A JSON Web Token (JWT) that securely communicates information about the user to the app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var identityToken: Data? { get }
```

## Discussion

The system encodes the object as a string using NSUTF8StringEncoding.

## See Also

### Identifying a User

var authorizationCode: Data?

A token that the app uses to interact with the server.

var state: String?

An arbitrary string that your app provides to the request that generates the credential.

var user: String

An identifier for the authenticated user.

