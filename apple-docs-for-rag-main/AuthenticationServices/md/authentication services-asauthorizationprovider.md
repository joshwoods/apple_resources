

- Authentication Services
-  ASAuthorizationProvider 

Protocol

# ASAuthorizationProvider

An interface that authorization providers must implement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol ASAuthorizationProvider : NSObjectProtocol
```

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- ASAuthorizationAppleIDProvider
- ASAuthorizationPasswordProvider
- ASAuthorizationPlatformPublicKeyCredentialProvider
- ASAuthorizationSecurityKeyPublicKeyCredentialProvider
- ASAuthorizationSingleSignOnProvider

## See Also

### Inspecting the Provider

var provider: any ASAuthorizationProvider

The provider servicing the request.

