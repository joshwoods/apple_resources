

- Authentication Services
- ASAuthorizationController
-  cancel() 

Instance Method

# cancel()

Cancels any active authorization requests.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 18.0+visionOS 1.0+

``` source
func cancel()
```

## Discussion

If calling this method cancels an active authorization request, the authorization controller calls its delegate’s authorizationController(controller:didCompleteWithError:) method.

## See Also

### Executing requests

func performRequests()

Starts the specified authorization flows during controller initialization.

func performRequests(options: ASAuthorizationController.RequestOptions)

Starts the specified authorization flows during controller initialization.

func performAutoFillAssistedRequests()

Initiates the authorization flows for requests that support AutoFill presentation.

struct RequestOptions

Options that modify how a controller performs authorization requests.

