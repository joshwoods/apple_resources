

- Authentication Services
- ASAuthorizationControllerDelegate
-  authorizationController(controller:didCompleteWithError:) 

Instance Method

# authorizationController(controller:didCompleteWithError:)

Tells the delegate when authorization fails, and provides an error explaining why.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor
optional func authorizationController(
    controller: ASAuthorizationController,
    didCompleteWithError error: any Error
)
```

## Parameters 

`controller`  

The controller that performs the authorization attempt.

`error`  

An error that explains the failure using one of the codes in ASAuthorizationError.Code.

## Mentioned in 

Supporting Security Key Authentication Using Physical Keys

Supporting passkeys

## See Also

### Handling Authorization Errors

let ASAuthorizationErrorDomain: String

The domain of authorization errors.

struct ASAuthorizationError

Errors that can occur during authorization.

