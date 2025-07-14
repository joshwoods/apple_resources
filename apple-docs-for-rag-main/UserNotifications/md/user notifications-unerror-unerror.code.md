

- User Notifications
- UNError
-  UNError.Code 

Enumeration

# UNError.Code

Constants that identify notification errors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum Code
```

## Topics

### Constants

case notificationsNotAllowed

Notifications aren’t allowed.

case attachmentInvalidURL

The URL for an attachment was invalid.

case attachmentUnrecognizedType

The file type of an attachment isn’t supported.

case attachmentInvalidFileSize

An attachment is too large.

case attachmentNotInDataStore

The specified attachment isn’t in the system data store.

case attachmentMoveIntoDataStoreFailed

An error occurred when trying to move an attachment to the system data store.

case attachmentCorrupt

The file for an attachment is corrupt.

case notificationInvalidNoDate

The notification doesn’t have an associated date, but should.

case notificationInvalidNoContent

The notification has no user-facing content, but should.

case contentProvidingInvalid

case contentProvidingObjectNotAllowed

### Enumeration Cases

case badgeInputInvalid

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

### Handling errors

struct UNError

An object that represents a notification error.

let UNErrorDomain: String

The error domain for notifications.

