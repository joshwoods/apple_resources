

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  isUserInterfaceEnabled 

Instance Property

# isUserInterfaceEnabled

Determines if user interface is available for the current request.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+visionOS 1.0+

``` source
var isUserInterfaceEnabled: Bool { get }
```

## Discussion

If this value is `false`, then calls to presentAuthorizationViewController(completion:) fail and the system cancels the request.

## See Also

### Interacting with the User

func presentAuthorizationViewController(completion: (Bool, (any Error)?) -> Void)

Asks the authorization service to show the extension’s view controller to the user.

