

- FamilyControls
-  FamilyControlsError 

Enumeration

# FamilyControlsError

Errors the Family Controls framework reports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+

``` source
enum FamilyControlsError
```

## Topics

### Error Values

case invalidAccountType

The device isn’t signed into a valid iCloud account.

case authorizationConflict

Another authorized app already provides parental controls.

case authorizationCanceled

The parent or guardian canceled a request for authorization.

case invalidArgument

The method’s arguments are invalid.

case unavailable

The system failed to set up the Family Control framework.

case restricted

A restriction prevents your app from using Family Controls on this device.

case networkError

The device must be connected to the network in order to enroll with parental controls.

case authenticationMethodUnavailable

The device must have a passcode set in order for an individual to enroll with parental controls.

### Error Data

var errorDescription: String?

A nonlocalized description of the error, suitable for debugging.

var errorDescription: String?

A nonlocalized description of the error, suitable for debugging.

var localizedDescription: String

Retrieve the localized description for this error.

var failureReason: String?

A localized message describing the reason for the failure.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

### Comparisons

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two error values aren’t equal.

func hash(into: inout Hasher)

var hashValue: Int

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- LocalizedError
- RawRepresentable
- Sendable

