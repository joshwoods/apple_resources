

- Authentication Services
-  ASAuthorizationControllerDelegate 

Protocol

# ASAuthorizationControllerDelegate

An interface for providing information about the outcome of an authorization request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor
protocol ASAuthorizationControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Supporting passkeys

Supporting Security Key Authentication Using Physical Keys

Authenticating people by using passkeys in browser apps

## Topics

### Handling Successful Authorization

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

func authorizationController(controller: ASAuthorizationController, didCompleteWithAuthorization: ASAuthorization)

Tells the delegate when authorization completes successfully.

class ASAuthorization

The encapsulation of a successful authorization by a controller.

### Handling Authorization Errors

func authorizationController(controller: ASAuthorizationController, didCompleteWithError: any Error)

Tells the delegate when authorization fails, and provides an error explaining why.

let ASAuthorizationErrorDomain: String

The domain of authorization errors.

struct ASAuthorizationError

Errors that can occur during authorization.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to request completion

var delegate: (any ASAuthorizationControllerDelegate)?

A delegate that the authorization controller informs about the success or failure of an authorization attempt.

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

