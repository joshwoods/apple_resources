

- Authentication Services
-  ASAuthorizationErrorDomain 

Global Variable

# ASAuthorizationErrorDomain

The domain of authorization errors.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let ASAuthorizationErrorDomain: String
```

## See Also

### Handling Authorization Errors

func authorizationController(controller: ASAuthorizationController, didCompleteWithError: any Error)

Tells the delegate when authorization fails, and provides an error explaining why.

struct ASAuthorizationError

Errors that can occur during authorization.

