

- PassKit (Apple Pay and Wallet)
-  PKDisbursementErrorDomain 

Global Variable

# PKDisbursementErrorDomain

The error domain to use for errors with in-app disbursements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
let PKDisbursementErrorDomain: String
```

## Discussion

Use the PKDisbursementErrorDomain to create your own PKDisbursementError objects, and return them to indicate problems with a transfer.

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

enum Code

Values that describe errors that can occur while processing the disbursement.

let PKPaymentErrorDomain: String

The error domain for specific errors associated with Apple Pay in-app or web payments.

