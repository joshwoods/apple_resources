

- Authentication Services
- ASAuthorizationSingleSignOnCredential
-  state 

Instance Property

# state

An arbitrary string that your app provided to the request that generated this credential.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var state: String? { get }
```

## See Also

### Identifying a User

var identityToken: Data?

A JSON Web Token (JWT) that securely communicates information about the user to your app.

var accessToken: Data?

An access token used to get an identity token.

var authorizedScopes: [ASAuthorization.Scope]

The contact information the user authorized your app to access.

