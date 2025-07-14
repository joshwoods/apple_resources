

- Authentication Services
- ASAuthorizationController
-  performAutoFillAssistedRequests() 

Instance Method

# performAutoFillAssistedRequests()

Initiates the authorization flows for requests that support AutoFill presentation.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
func performAutoFillAssistedRequests()
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

Supporting passkeys

## Discussion

The authorization controller presents a user interface when a text field with the appropriate text content type obtains focus.

Upon completion, the authorization controller calls its delegate to report success or failure.

## See Also

### Executing requests

func performRequests()

Starts the specified authorization flows during controller initialization.

func performRequests(options: ASAuthorizationController.RequestOptions)

Starts the specified authorization flows during controller initialization.

func cancel()

Cancels any active authorization requests.

struct RequestOptions

Options that modify how a controller performs authorization requests.

