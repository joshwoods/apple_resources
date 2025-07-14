

- User Notifications
- UNError
- UNError.Code
-  UNError.Code.notificationsNotAllowed 

Case

# UNError.Code.notificationsNotAllowed

Notifications aren’t allowed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case notificationsNotAllowed
```

## Discussion

This error occurs when you try to submit a notification request and your app or app extension isn’t authorized to schedule notifications.

## See Also

### Constants

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

