

- Foundation
- NSNotification
- NSNotification.Name
-  CKAccountChanged 

Type Property

# CKAccountChanged

A notification that a container posts when the status of an iCloud account changes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
static let CKAccountChanged: NSNotification.Name
```

## Discussion

Create an instance of CKContainer to receive this notification. The container posts the notification using an arbitrary queue. Use the accountStatus(completionHandler:) method to obtain the account’s status.

