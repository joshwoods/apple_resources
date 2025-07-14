

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  presentAuthorizationViewController(completion:) 

Instance Method

# presentAuthorizationViewController(completion:)

Asks the authorization service to show the extension’s view controller to the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
func presentAuthorizationViewController(completion: @escaping (Bool, (any Error)?) -> Void)
```

``` source
func presentAuthorizationViewController() async throws
```

## Parameters 

`completion`  

A completion handler that the method uses to indicate whether the view controller was presented successfully, and the specific error if not.

## Discussion

This is only valid during authentication requests. If the system can’t show the controller, the completion returns an error.

## See Also

### Interacting with the User

var isUserInterfaceEnabled: Bool

Determines if user interface is available for the current request.

