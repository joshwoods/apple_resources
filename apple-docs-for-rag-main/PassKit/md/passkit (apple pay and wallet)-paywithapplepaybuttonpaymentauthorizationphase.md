

- PassKit (Apple Pay and Wallet)
-  PayWithApplePayButtonPaymentAuthorizationPhase 

Enumeration

# PayWithApplePayButtonPaymentAuthorizationPhase

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+visionOSwatchOS 9.0+

``` source
enum PayWithApplePayButtonPaymentAuthorizationPhase
```

## Topics

### Enumeration Cases

case didAuthorize(payment: PKPayment, resultHandler: (PKPaymentAuthorizationResult) -> Void)

case didFinish

case willAuthorize

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

enum PKVehicleConnectionErrorCode

let PKPassKitErrorDomain: String

The error domain for PassKit errors.

let PKIdentityErrorDomain: String

The error domain for identity errors.

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

let PKShareSecureElementPassErrorDomain: String

