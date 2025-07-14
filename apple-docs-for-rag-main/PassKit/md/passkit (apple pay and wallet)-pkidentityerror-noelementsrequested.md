

- PassKit (Apple Pay and Wallet)
- PKIdentityError
-  noElementsRequested 

Type Property

# noElementsRequested

An error that indicates the elements aren’t supported.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var noElementsRequested: PKIdentityError.Code { get }
```

## See Also

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

static var requestAlreadyInProgress: PKIdentityError.Code

An error that indicates a request is already in progress.

static var unknown: PKIdentityError.Code

An error that indicates an unknown error.

