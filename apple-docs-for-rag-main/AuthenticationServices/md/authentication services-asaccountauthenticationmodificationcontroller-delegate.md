

- Authentication Services
- ASAccountAuthenticationModificationController
-  delegate 

Instance Property

# delegate

An object that receives notifications about the request’s status.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
weak var delegate: (any ASAccountAuthenticationModificationControllerDelegate)? { get set }
```

## See Also

### Configuring Requests

var presentationContextProvider: (any ASAccountAuthenticationModificationControllerPresentationContextProviding)?

An object that provides a presentation context for the account modification request’s user interface.

