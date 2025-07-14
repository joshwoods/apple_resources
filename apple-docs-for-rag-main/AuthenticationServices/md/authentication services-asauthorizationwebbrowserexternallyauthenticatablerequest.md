

- Authentication Services
-  ASAuthorizationWebBrowserExternallyAuthenticatableRequest 

Protocol

# ASAuthorizationWebBrowserExternallyAuthenticatableRequest

An authorization request for which a web browser can retrieve credentials.

macOS 13.3+

``` source
protocol ASAuthorizationWebBrowserExternallyAuthenticatableRequest : NSObjectProtocol
```

## Topics

### Local authentication

var authenticatedContext: LAContext?

The local authentication context for the authorization.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

## See Also

### Website authentication requests

protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialAssertionRequest

An interface you use to respond to authentication challenges in a web browser.

protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest

An interface you use to respond to passkey-creation challenges in a web browser.

