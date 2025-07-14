

- PassKit (Apple Pay and Wallet)
- PKDisbursementError
-  PKDisbursementError.Code 

Enumeration

# PKDisbursementError.Code

Values that describe errors that can occur while processing the disbursement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case recipientContactInvalidError

The recipient’s contact information wasn’t valid.

case unsupportedCardError

The framework doesn’t support the card the individual presented.

case unknownError

An unknown error occurred.

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

struct PKDisbursementError

A structure that describes errors that can occur while processing the disbursement.

struct PKDisbursementErrorKey

Values that describe errors that can occur when processing disbursements.

struct PKPaymentError

An error type that you create to indicate problems with address or contact information on an Apple Pay sheet.

enum Code

An error code that you provide to indicate problems with address or contact information on an Apple Pay sheet.

struct PKPaymentErrorKey

Additional details about an error on the Apple Pay sheet.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

