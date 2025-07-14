

- Authentication Services
- ASAuthorizationController
-  ASAuthorizationController.RequestOptions 

Structure

# ASAuthorizationController.RequestOptions

Options that modify how a controller performs authorization requests.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct RequestOptions
```

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var preferImmediatelyAvailableCredentials: ASAuthorizationController.RequestOptions

Tells the authorization controller to prefer credentials that are immediately available on the local device.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Executing requests

func performRequests()

Starts the specified authorization flows during controller initialization.

func performRequests(options: ASAuthorizationController.RequestOptions)

Starts the specified authorization flows during controller initialization.

func performAutoFillAssistedRequests()

Initiates the authorization flows for requests that support AutoFill presentation.

func cancel()

Cancels any active authorization requests.

