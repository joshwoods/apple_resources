

- Authentication Services
-  ASAuthorizationResult 

Enumeration

# ASAuthorizationResult

Describes the outcome of a successful authorization request.

AuthenticationServicesSwiftUIiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
enum ASAuthorizationResult
```

## Topics

### Authorization results

case appleID(ASAuthorizationAppleIDCredential)

A credential from an Apple ID authentication.

case customMethod(ASAuthorizationCustomMethod)

A chosen custom authorization method.

case passkeyAssertion(ASAuthorizationPlatformPublicKeyCredentialAssertion)

A passkey credential from an assertion request.

case passkeyRegistration(ASAuthorizationPlatformPublicKeyCredentialRegistration)

A new passkey credential from a registration request.

case password(ASPasswordCredential)

A password credential.

case securityKeyAssertion(ASAuthorizationSecurityKeyPublicKeyCredentialAssertion)

A security key credential from an assertion request.

case securityKeyRegistration(ASAuthorizationSecurityKeyPublicKeyCredentialRegistration)

A new security key credential from a registration request.

## Relationships

### Conforms To

- Sendable

## See Also

### Authorization requests

class ASAuthorizationController

A controller that manages authorization requests that a provider creates.

struct AuthorizationController

A SwiftUI environment value that views use to perform authorization requests.

