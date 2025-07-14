

- Authentication Services
- ASAuthorization
- ASAuthorization.OpenIDOperation
-  operationLogout 

Type Property

# operationLogout

An operation that ends an authenticated session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let operationLogout: ASAuthorization.OpenIDOperation
```

## See Also

### Operation Types

static let operationLogin: ASAuthorization.OpenIDOperation

An operation used to authenticate a user.

static let operationRefresh: ASAuthorization.OpenIDOperation

An operation that refreshes the logged-in user’s credentials.

static let operationImplicit: ASAuthorization.OpenIDOperation

An operation that depends on the particular kind of credential provider.

