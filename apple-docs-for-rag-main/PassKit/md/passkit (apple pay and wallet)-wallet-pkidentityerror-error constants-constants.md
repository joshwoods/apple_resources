

- PassKit (Apple Pay and Wallet)
- Wallet
- PKIdentityError
-  Error constants 

API Collection

# Error constants

Error code constants for identity operations.

## Topics

### Constants

static var cancelled: PKIdentityError.Code

An error that indicates the user cancels the presented sheet.

static var invalidElement: PKIdentityError.Code

An error that indicates an element the app requests isn’t valid.

static var invalidNonce: PKIdentityError.Code

An error that indicates the number is too large or unsuitable.

static var notSupported: PKIdentityError.Code

An error that indicates the request originates from a device the framework doesn’t support.

static var networkUnavailable: PKIdentityError.Code

An error that indicates a network isn’t available.

static var noElementsRequested: PKIdentityError.Code

An error that indicates the elements aren’t supported.

static var requestAlreadyInProgress: PKIdentityError.Code

An error that indicates a request is already in progress.

static var unknown: PKIdentityError.Code

An error that indicates an unknown error.

## See Also

### Inspecting an error

var code: Code

The error code.

enum Code

Error codes for identity operations.

var errorCode: Int

The integer error code.

var userInfo: [String : Any]

The user information for the error.

var errorUserInfo: [String : Any]

The error user information dictionary for the error.

