

- Authentication Services
-  ASAuthorizationRequest 

Class

# ASAuthorizationRequest

A base class for different kinds of authorization requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationRequest
```

## Overview

Use one of the concrete requests, like ASAuthorizationAppleIDRequest, ASAuthorizationPasswordRequest, or ASAuthorizationSingleSignOnRequest.

You typically generate one of these using the corresponding provider, which is an instance of ASAuthorizationAppleIDProvider, ASAuthorizationPasswordProvider, or ASAuthorizationSingleSignOnProvider, respectively.

## Topics

### Inspecting the Provider

var provider: any ASAuthorizationProvider

The provider servicing the request.

protocol ASAuthorizationProvider

An interface that authorization providers must implement.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ASAuthorizationOpenIDRequest
- ASAuthorizationPasswordRequest
- ASAuthorizationPlatformPublicKeyCredentialAssertionRequest
- ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
- ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Inspecting requests

var authorizationRequests: [ASAuthorizationRequest]

The authorization requests that the controller manages.

var customAuthorizationMethods: [ASAuthorizationCustomMethod]

An array of custom authorization methods for the user to choose.

