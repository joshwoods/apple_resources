

- PassKit (Apple Pay and Wallet)
-  PKDisbursementError 

Structure

# PKDisbursementError

A structure that describes errors that can occur while processing the disbursement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
struct PKDisbursementError
```

## Topics

### Initializers

init(Code, userInfo: [String : Any])

Creates a new error structure with the error code and user info you provide.

### Error details

var code: Code

The code that describes the error.

enum Code

Values that describe errors that can occur while processing the disbursement.

var errorCode: Int

An integer value that represents the error code.

var errorUserInfo: [String : Any]

A dictionary that contains additional details about the error.

var hashValue: Int

The hash value.

var userInfo: [String : Any]

A dictionary that contains additional details about the error.

### Type properties

static var recipientContactInvalidError: PKDisbursementError.Code

A value that indicates the recipient’s contact information is invalid.

static var unknownError: PKDisbursementError.Code

A value that indicates an unknown error occurred.

static var unsupportedCardError: PKDisbursementError.Code

A value that indicates that the framework doesn’t support the card the individual presented for this disbursement.

### Utility methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func == (PKDisbursementError, PKDisbursementError) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

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

let PKDisbursementErrorDomain: String

The error domain to use for errors with in-app disbursements.

