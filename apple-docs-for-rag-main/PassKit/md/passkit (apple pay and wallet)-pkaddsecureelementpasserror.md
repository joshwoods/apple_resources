

- PassKit (Apple Pay and Wallet)
-  PKAddSecureElementPassError 

Structure

# PKAddSecureElementPassError

An error object that PassKit uses when it adds Secure Element passes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+watchOS 6.2+

``` source
struct PKAddSecureElementPassError
```

## Topics

### Creating a secure element pass error object

init(Code, userInfo: [String : Any])

Creates a Secure Element payment pass error object of the specified type with the specified user information.

### Identifying errors

static var deviceNotReadyError: PKAddSecureElementPassError.Code

The device isn’t ready to add Secure Element passes.

static var deviceNotSupportedError: PKAddSecureElementPassError.Code

The device doesn’t support adding Secure Element passes.

static var invalidConfigurationError: PKAddSecureElementPassError.Code

An error that occurs when they system attempts to add a Secure Element pass using an invalid configuration.

static var unavailableError: PKAddSecureElementPassError.Code

PassKit is temporarily unable to add Secure Element passes.

static var unknownError: PKAddSecureElementPassError.Code

An error that occurs when PassKit cancels the addition of a Secure Element pass due to an unknown failure.

Deprecated

static var userCanceledError: PKAddSecureElementPassError.Code

An error that occurs when the user cancels the addition of a Secure Element pass.

enum Code

Error codes for problems that occur when you add a secure element passes.

### Getting error information

var code: Code

The code that provides context for the error.

var errorCode: Int

The code that provides context for the error.

var userInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

var errorUserInfo: [String : Any]

A dictionary that contains custom information that relates to the error.

let PKAddSecureElementPassErrorDomain: String

The error domain for errors that occur when adding a secure pass.

### Comparing errors

static func == (PKAddSecureElementPassError, PKAddSecureElementPassError) -> Bool

Returns a Boolean value that indicates whether the two add secure element pass errors are equal.

### Hashing

func hash(into: inout Hasher)

Hashes the Secure Element pass error object by feeding the item into the given hasher.

var hashValue: Int

The hash value for the Secure Element pass error.

### Type Properties

static var errorDomain: String

static var genericError: PKAddSecureElementPassError.Code

static var osVersionNotSupportedError: PKAddSecureElementPassError.Code

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

struct PKPassKitError

Errors that the PassKit framework uses.

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

