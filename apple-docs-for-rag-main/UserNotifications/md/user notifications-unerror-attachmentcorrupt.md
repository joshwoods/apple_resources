

- User Notifications
- UNError
-  attachmentCorrupt 

Type Property

# attachmentCorrupt

The file for an attachment is corrupt.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static var attachmentCorrupt: UNError.Code { get }
```

## See Also

### Type Properties

static var notificationsNotAllowed: UNError.Code

Notifications are not allowed.

static var attachmentInvalidURL: UNError.Code

The URL for an attachment was invalid.

static var attachmentUnrecognizedType: UNError.Code

The file type of an attachment is not supported.

static var attachmentInvalidFileSize: UNError.Code

An attachment is too large.

static var attachmentNotInDataStore: UNError.Code

The specified attachment is not in the system data store.

static var attachmentMoveIntoDataStoreFailed: UNError.Code

An error occurred when trying to move an attachment to the system data store.

static var notificationInvalidNoDate: UNError.Code

The notification does not have an associated date, but should.

static var notificationInvalidNoContent: UNError.Code

The notification has no user-facing content, but should.

static var contentProvidingInvalid: UNError.Code

static var contentProvidingObjectNotAllowed: UNError.Code

static var badgeInputInvalid: UNError.Code

