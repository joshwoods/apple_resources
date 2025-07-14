

- Authentication Services
- ASAuthorizationController
-  delegate 

Instance Property

# delegate

A delegate that the authorization controller informs about the success or failure of an authorization attempt.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
weak var delegate: (any ASAuthorizationControllerDelegate)? { get set }
```

## See Also

### Responding to request completion

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

protocol ASAuthorizationControllerDelegate

An interface for providing information about the outcome of an authorization request.

