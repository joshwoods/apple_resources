

- PassKit (Apple Pay and Wallet)
-  PKIdentityError 

Structure

# PKIdentityError

A structure that represents an identity error.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct PKIdentityError
```

## Topics

### Inspecting an error

var code: Code

The error code.

enum Code

Error codes for identity operations.

Error constants

Error code constants for identity operations.

var errorCode: Int

The integer error code.

var userInfo: [String : Any]

The user information for the error.

var errorUserInfo: [String : Any]

The error user information dictionary for the error.

### Comparing errors

static func == (PKIdentityError, PKIdentityError) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Accessing the hash value

func hash(into: inout Hasher)

Hashes the essential components of the value by passing them into the hasher.

var hashValue: Int

The hash value.

### Creating an identity error

init(Code, userInfo: [String : Any])

Creates an identity error with an error code and user information.

### Type Properties

static var errorDomain: String

static var regionNotSupported: PKIdentityError.Code

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

struct PKAddSecureElementPassError

An error object that PassKit uses when it adds Secure Element passes.

enum Code

Errors that the PassKit framework uses.

enum Code

Error codes for problems that occur when you add a secure element passes.

enum PKAddPaymentPassError

Error codes for adding payment passes.

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

