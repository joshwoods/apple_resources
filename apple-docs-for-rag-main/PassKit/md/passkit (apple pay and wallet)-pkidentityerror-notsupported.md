

- PassKit (Apple Pay and Wallet)
- PKIdentityError
-  notSupported 

Type Property

# notSupported

An error that indicates the request originates from a device the framework doesn’t support.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var notSupported: PKIdentityError.Code { get }
```

## See Also

### Constants

static var cancelled: PKIdentityError.Code

An error that indicates the user cancels the presented sheet.

static var invalidElement: PKIdentityError.Code

An error that indicates an element the app requests isn’t valid.

static var invalidNonce: PKIdentityError.Code

An error that indicates the number is too large or unsuitable.

static var networkUnavailable: PKIdentityError.Code

An error that indicates a network isn’t available.

static var noElementsRequested: PKIdentityError.Code

An error that indicates the elements aren’t supported.

static var requestAlreadyInProgress: PKIdentityError.Code

An error that indicates a request is already in progress.

static var unknown: PKIdentityError.Code

An error that indicates an unknown error.

