

- Authentication Services
- ASAuthorization
-  ASAuthorization.OpenIDOperation 

Structure

# ASAuthorization.OpenIDOperation

The kinds of operations that you can perform with OpenID authentication.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct OpenIDOperation
```

## Discussion

Use one of these values as the requestedOperation property in an OpenID request that you make with an instance of either ASAuthorizationAppleIDRequest or ASAuthorizationSingleSignOnRequest.

## Topics

### Operation Types

static let operationLogin: ASAuthorization.OpenIDOperation

An operation used to authenticate a user.

static let operationRefresh: ASAuthorization.OpenIDOperation

An operation that refreshes the logged-in user’s credentials.

static let operationLogout: ASAuthorization.OpenIDOperation

An operation that ends an authenticated session.

static let operationImplicit: ASAuthorization.OpenIDOperation

An operation that depends on the particular kind of credential provider.

### Creating an Operation

init(String)

Creates an operation from the given string.

init(rawValue: String)

Creates an operation from the given string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the Operation

var requestedOperation: ASAuthorization.OpenIDOperation

The OpenID authentication operation you want this request to perform.

