

- PassKit (Apple Pay and Wallet)
-  PKDisbursementErrorKey 

Structure

# PKDisbursementErrorKey

Values that describe errors that can occur when processing disbursements.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKDisbursementErrorKey
```

## Topics

### Initializers

init(rawValue: String)

Create a new disbursement error key with the provided value.

### Type properties

static let contactFieldUserInfoKey: PKDisbursementErrorKey

The contact field the error relates to.

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

struct PKPaymentError

An error type that you create to indicate problems with address or contact information on an Apple Pay sheet.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

struct PKPaymentErrorKey

Additional details about an error on the Apple Pay sheet.

enum Code

Values that describe errors that can occur while processing the disbursement.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

