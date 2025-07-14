

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassError
- PKAddSecureElementPassError.Code
-  PKAddSecureElementPassError.Code.genericError 

Case

# PKAddSecureElementPassError.Code.genericError

Represents the default error case.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+watchOS 11.0+

``` source
case genericError
```

## See Also

### Error codes

case deviceNotReadyError

The reader for the pass isn’t ready to start pairing.

case deviceNotSupportedError

The reader for the pass isn’t supported or has an invalid version.

case invalidConfigurationError

The configuration for the pass is invalid for either Wallet or the reader.

case osVersionNotSupportedError

case unavailableError

Provisioning for secure element passes isn’t available on the device, or the app is missing the entitlement.

case userCanceledError

The user canceled adding the pass.

static var unknownError: PKAddSecureElementPassError.CodeDeprecated

