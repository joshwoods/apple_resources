

- Authentication Services
- ASAuthorization
- ASAuthorization.OpenIDOperation
-  operationRefresh 

Type Property

# operationRefresh

An operation that refreshes the logged-in user’s credentials.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let operationRefresh: ASAuthorization.OpenIDOperation
```

## See Also

### Operation Types

static let operationLogin: ASAuthorization.OpenIDOperation

An operation used to authenticate a user.

static let operationLogout: ASAuthorization.OpenIDOperation

An operation that ends an authenticated session.

static let operationImplicit: ASAuthorization.OpenIDOperation

An operation that depends on the particular kind of credential provider.

