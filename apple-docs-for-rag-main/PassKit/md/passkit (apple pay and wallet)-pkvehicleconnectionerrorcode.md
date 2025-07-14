

- PassKit (Apple Pay and Wallet)
-  PKVehicleConnectionErrorCode 

Enumeration

# PKVehicleConnectionErrorCode

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOSvisionOS 1.0+watchOS 8.5+

``` source
enum PKVehicleConnectionErrorCode
```

## Topics

### Enumeration Cases

case sessionNotActive

case sessionUnableToStart

case unknown

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

enum Code

Error codes for problems that occur when you add a secure element passes.

enum PKAddPaymentPassError

Error codes for adding payment passes.

struct PKIdentityError

A structure that represents an identity error.

enum Code

Error codes for identity operations.

struct PKShareSecureElementPassError

enum Code

enum PayWithApplePayButtonPaymentAuthorizationPhase

let PKPassKitErrorDomain: String

The error domain for PassKit errors.

let PKIdentityErrorDomain: String

The error domain for identity errors.

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

let PKShareSecureElementPassErrorDomain: String

