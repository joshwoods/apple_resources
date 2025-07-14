

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassError
- PKAddSecureElementPassError.Code
-  PKAddSecureElementPassError.Code.deviceNotReadyError 

Case

# PKAddSecureElementPassError.Code.deviceNotReadyError

The reader for the pass isn’t ready to start pairing.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+watchOS 6.2+

``` source
case deviceNotReadyError
```

## See Also

### Error codes

case deviceNotSupportedError

The reader for the pass isn’t supported or has an invalid version.

case genericError

Represents the default error case.

case invalidConfigurationError

The configuration for the pass is invalid for either Wallet or the reader.

case osVersionNotSupportedError

case unavailableError

Provisioning for secure element passes isn’t available on the device, or the app is missing the entitlement.

case userCanceledError

The user canceled adding the pass.

static var unknownError: PKAddSecureElementPassError.CodeDeprecated

