

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassError
-  PKAddSecureElementPassError.Code 

Enumeration

# PKAddSecureElementPassError.Code

Error codes for problems that occur when you add a secure element passes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+watchOS 6.2+

``` source
enum Code
```

## Topics

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

static var unknownError: PKAddSecureElementPassError.CodeDeprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct PKPassKitError

Errors that the PassKit framework uses.

struct PKAddSecureElementPassError

An error object that PassKit uses when it adds Secure Element passes.

enum Code

Errors that the PassKit framework uses.

enum PKAddPaymentPassError

Error codes for adding payment passes.

struct PKIdentityError

A structure that represents an identity error.

enum Code

Error codes for identity operations.

struct PKShareSecureElementPassError

enum Code

enum PKVehicleConnectionErrorCode

enum PayWithApplePayButtonPaymentAuthorizationPhase

let PKPassKitErrorDomain: String

The error domain for PassKit errors.

let PKIdentityErrorDomain: String

The error domain for identity errors.

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

let PKShareSecureElementPassErrorDomain: String

