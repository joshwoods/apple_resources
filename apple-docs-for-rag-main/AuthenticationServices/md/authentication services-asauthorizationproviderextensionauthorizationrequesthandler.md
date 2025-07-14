

- Authentication Services
-  ASAuthorizationProviderExtensionAuthorizationRequestHandler 

Protocol

# ASAuthorizationProviderExtensionAuthorizationRequestHandler

An interface through which a single sign-on (SSO) authentication provider extension handles authentication requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
protocol ASAuthorizationProviderExtensionAuthorizationRequestHandler : NSObjectProtocol
```

## Topics

### Starting or Canceling a Request

func beginAuthorization(with: ASAuthorizationProviderExtensionAuthorizationRequest)

Tells your request handler to authorize the given request.

**Required**

func cancelAuthorization(with: ASAuthorizationProviderExtensionAuthorizationRequest)

Tells your request handler to cancel the authorization of the given request.

class ASAuthorizationProviderExtensionAuthorizationRequest

An authorization request that your provider extension handles.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Performing enterprise single sign-on

class ASAuthorizationSingleSignOnProvider

A mechanism for generating requests to authenticate users with third-party providers.

class ASAuthorizationSingleSignOnCredential

A credential that results from a successful single sign-on (SSO) authentication.

class ASAuthorizationProviderExtensionAuthorizationResult

The result of an authorization request.

struct RequestOptions

Options that modify how a controller performs authorization requests.

