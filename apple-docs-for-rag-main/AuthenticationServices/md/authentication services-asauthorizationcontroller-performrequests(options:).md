

- Authentication Services
- ASAuthorizationController
-  performRequests(options:) 

Instance Method

# performRequests(options:)

Starts the specified authorization flows during controller initialization.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func performRequests(options: ASAuthorizationController.RequestOptions = [])
```

## See Also

### Executing requests

func performRequests()

Starts the specified authorization flows during controller initialization.

func performAutoFillAssistedRequests()

Initiates the authorization flows for requests that support AutoFill presentation.

func cancel()

Cancels any active authorization requests.

struct RequestOptions

Options that modify how a controller performs authorization requests.

