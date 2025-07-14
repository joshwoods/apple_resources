

- Authentication Services
- ASAuthorizationSingleSignOnProvider
-  canPerformAuthorization 

Instance Property

# canPerformAuthorization

A Boolean value that indicates if the provider is capable of performing authorization within a given configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var canPerformAuthorization: Bool { get }
```

## See Also

### Creating Authorization Requests

func createRequest() -> ASAuthorizationSingleSignOnRequest

Creates a single sign-on (SSO) authorization request.

class ASAuthorizationSingleSignOnRequest

An OpenID authorization request that provides single sign-on (SSO) functionality.

class ASAuthorizationOpenIDRequest

An OpenID authorization request.

