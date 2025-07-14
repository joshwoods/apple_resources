

- PassKit (Apple Pay and Wallet)
- PKIdentityError
-  PKIdentityError.Code 

Enumeration

# PKIdentityError.Code

Error codes for identity operations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Error codes

case cancelled

An error that indicates the user cancels the presented sheet.

case invalidElement

An error that indicates an element the app requests isn’t valid.

case invalidNonce

An error that indicates the number is too large or unsuitable.

case notSupported

An error that indicates the request originates from a device the framework doesn’t support.

case networkUnavailable

An error that indicates a network isn’t available.

case noElementsRequested

An error that indicates the elements aren’t supported.

case requestAlreadyInProgress

An error that indicates a request is already in progress.

case unknown

An error that indicates an unknown error.

### Enumeration Cases

case regionNotSupported

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

