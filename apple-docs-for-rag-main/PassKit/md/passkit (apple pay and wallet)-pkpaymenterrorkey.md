

- PassKit (Apple Pay and Wallet)
-  PKPaymentErrorKey 

Structure

# PKPaymentErrorKey

Additional details about an error on the Apple Pay sheet.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKPaymentErrorKey
```

## Discussion

Use payment error keys if you are creating a payment error without using one of the convenience methods in PKPaymentRequest (such as paymentBillingAddressInvalidError(withKey:localizedDescription:) or others).

The payment error keys indicate a specific field that has an error, for example, the street field of an address.

## Topics

### Initializing a payment error key

init(rawValue: String)

Create an error key given the raw value.

### Error keys

static let postalAddressUserInfoKey: PKPaymentErrorKey

Payment error key that indicates errors with the postal address.

static let contactFieldUserInfoKey: PKPaymentErrorKey

Payment error key that indicates errors with the contact information.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct PKDisbursementError

A structure that describes errors that can occur while processing the disbursement.

struct PKDisbursementErrorKey

Values that describe errors that can occur when processing disbursements.

struct PKPaymentError

An error type that you create to indicate problems with address or contact information on an Apple Pay sheet.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

enum Code

Values that describe errors that can occur while processing the disbursement.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

