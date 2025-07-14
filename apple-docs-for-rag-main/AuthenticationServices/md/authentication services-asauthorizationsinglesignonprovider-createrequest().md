

- Authentication Services
- ASAuthorizationSingleSignOnProvider
-  createRequest() 

Instance Method

# createRequest()

Creates a single sign-on (SSO) authorization request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func createRequest() -> ASAuthorizationSingleSignOnRequest
```

## Return Value

A single sign-on (SSO) authorization request.

## See Also

### Creating Authorization Requests

var canPerformAuthorization: Bool

A Boolean value that indicates if the provider is capable of performing authorization within a given configuration.

class ASAuthorizationSingleSignOnRequest

An OpenID authorization request that provides single sign-on (SSO) functionality.

class ASAuthorizationOpenIDRequest

An OpenID authorization request.

