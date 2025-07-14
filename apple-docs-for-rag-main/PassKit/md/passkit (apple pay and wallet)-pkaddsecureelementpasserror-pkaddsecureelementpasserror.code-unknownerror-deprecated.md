

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassError
- PKAddSecureElementPassError.Code
-  unknownError Deprecated

Type Property

# unknownError

iOS 13.4–18.0DeprecatediPadOS 13.4–18.0DeprecatedMac Catalyst 13.4–18.0DeprecatedmacOSvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
static var unknownError: PKAddSecureElementPassError.Code { get }
```

Deprecated

Use PKAddSecureElementPassGeneralError instead.

## See Also

### Error codes

case deviceNotReadyError

The reader for the pass isn’t ready to start pairing.

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

