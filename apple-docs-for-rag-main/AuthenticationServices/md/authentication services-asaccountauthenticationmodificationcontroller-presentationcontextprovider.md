

- Authentication Services
- ASAccountAuthenticationModificationController
-  presentationContextProvider 

Instance Property

# presentationContextProvider

An object that provides a presentation context for the account modification request’s user interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
weak var presentationContextProvider: (any ASAccountAuthenticationModificationControllerPresentationContextProviding)? { get set }
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## See Also

### Configuring Requests

var delegate: (any ASAccountAuthenticationModificationControllerDelegate)?

An object that receives notifications about the request’s status.

