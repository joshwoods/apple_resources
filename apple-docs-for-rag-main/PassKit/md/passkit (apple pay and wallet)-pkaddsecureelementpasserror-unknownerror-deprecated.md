

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassError
-  unknownError Deprecated

Type Property

# unknownError

An error that occurs when PassKit cancels the addition of a Secure Element pass due to an unknown failure.

iOS 13.4–18.0DeprecatediPadOS 13.4–18.0DeprecatedMac Catalyst 13.4–18.0DeprecatedmacOSvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
static var unknownError: PKAddSecureElementPassError.Code { get }
```

Deprecated

Use PKAddSecureElementPassGeneralError instead.

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

static var userCanceledError: PKAddSecureElementPassError.Code

An error that occurs when the user cancels the addition of a Secure Element pass.

enum Code

Error codes for problems that occur when you add a secure element passes.

