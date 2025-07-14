

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassError
-  userCanceledError 

Type Property

# userCanceledError

An error that occurs when the user cancels the addition of a Secure Element pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+watchOS 6.2+

``` source
static var userCanceledError: PKAddSecureElementPassError.Code { get }
```

## See Also

### Identifying errors

static var deviceNotReadyError: PKAddSecureElementPassError.Code

The device isn’t ready to add Secure Element passes.

static var deviceNotSupportedError: PKAddSecureElementPassError.Code

The device doesn’t support adding Secure Element passes.

static var invalidConfigurationError: PKAddSecureElementPassError.Code

An error that occurs when they system attempts to add a Secure Element pass using an invalid configuration.

static var unavailableError: PKAddSecureElementPassError.Code

PassKit is temporarily unable to add Secure Element passes.

static var unknownError: PKAddSecureElementPassError.Code

An error that occurs when PassKit cancels the addition of a Secure Element pass due to an unknown failure.

Deprecated

enum Code

Error codes for problems that occur when you add a secure element passes.

