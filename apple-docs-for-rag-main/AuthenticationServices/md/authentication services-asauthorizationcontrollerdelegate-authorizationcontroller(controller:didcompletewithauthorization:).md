

- Authentication Services
- ASAuthorizationControllerDelegate
-  authorizationController(controller:didCompleteWithAuthorization:) 

Instance Method

# authorizationController(controller:didCompleteWithAuthorization:)

Tells the delegate when authorization completes successfully.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor
optional func authorizationController(
    controller: ASAuthorizationController,
    didCompleteWithAuthorization authorization: ASAuthorization
)
```

## Parameters 

`controller`  

The controller that performs the authorization request.

`authorization`  

An encapsulation of the successful authorization.

## Mentioned in 

Supporting Security Key Authentication Using Physical Keys

Supporting passkeys

## See Also

### Handling Successful Authorization

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

class ASAuthorization

The encapsulation of a successful authorization by a controller.

