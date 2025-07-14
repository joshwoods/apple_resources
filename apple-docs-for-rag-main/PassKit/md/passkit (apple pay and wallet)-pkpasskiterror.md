

- PassKit (Apple Pay and Wallet)
-  PKPassKitError 

Structure

# PKPassKitError

Errors that the PassKit framework uses.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
struct PKPassKitError
```

## Topics

### Creating a pass error object

init(Code, userInfo: [String : Any])

Creates a pass error object of the specified type with the specified user information.

### Error information

var code: Code

The code that provides context for the error.

var errorCode: Int

The code that provides context for the error.

var userInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

var errorUserInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

### Error codes

static var invalidDataError: PKPassKitError.Code

static var invalidSignature: PKPassKitError.Code

static var notEntitledError: PKPassKitError.Code

static var unknownError: PKPassKitError.Code

static var unsupportedVersionError: PKPassKitError.Code

enum Code

Errors that the PassKit framework uses.

enum PKAddPaymentPassError

Error codes for adding payment passes.

### Error domain

let PKPassKitErrorDomain: String

The error domain for PassKit errors.

### Comparison operator

static func == (PKPassKitError, PKPassKitError) -> Bool

Returns a Boolean value indicating whether two pass error objects are equal.

### Hashing

func hash(into: inout Hasher)

Hashes the pass error object by feeding the item into the given hasher.

var hashValue: Int

The hash value for the Secure Element pass error.

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

enum PayWithApplePayButtonPaymentAuthorizationPhase

let PKPassKitErrorDomain: String

The error domain for PassKit errors.

let PKIdentityErrorDomain: String

The error domain for identity errors.

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

let PKShareSecureElementPassErrorDomain: String

