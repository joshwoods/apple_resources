

- PassKit (Apple Pay and Wallet)
- PKPassKitError
-  PKPassKitError.Code 

Enumeration

# PKPassKitError.Code

Errors that the PassKit framework uses.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
enum Code
```

## Topics

### Error codes

case unknownError

Unknown error.

case invalidDataError

Invalid pass data.

case unsupportedVersionError

Unsupported pass version.

case invalidSignature

Invalid pass signature.

case notEntitledError

Error caused by absence of the required entitlements for the given operation.

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

Error codes for problems that occur when you add a secure element passes.

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

