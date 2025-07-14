

- Authentication Services
- ASAuthorizationController
-  performRequests() 

Instance Method

# performRequests()

Starts the specified authorization flows during controller initialization.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func performRequests()
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

Supporting passkeys

## Discussion

When authorization succeeds, the system relays that information to the controller’s delegate by calling the authorizationController(controller:didCompleteWithAuthorization:) method with an authorization instance. If authorization fails, the system calls the authorizationController(controller:didCompleteWithError:) method instead.

Some authorization flows require a presentation context to ask the user for information or consent. Adopt the `ASAuthorizationControllerPresenting` protocol in one of your app’s classes, and set an instance of that class as the authorization controller’s `presentationController`.

## See Also

### Executing requests

func performRequests(options: ASAuthorizationController.RequestOptions)

Starts the specified authorization flows during controller initialization.

func performAutoFillAssistedRequests()

Initiates the authorization flows for requests that support AutoFill presentation.

func cancel()

Cancels any active authorization requests.

struct RequestOptions

Options that modify how a controller performs authorization requests.

