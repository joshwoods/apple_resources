

- Foundation
- UserDefaults
-  noCloudAccountNotification 

Type Property

# noCloudAccountNotification

Posted when a cloud default is set, but no iCloud user is logged in.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let noCloudAccountNotification: NSNotification.Name
```

## Discussion

This notification is posted to the default notification center on the main queue.

This notification doesn’t necessarily indicate an error; ubiquitous defaults set when no iCloud user is logged in are uploaded the next time one is available if configured to do so.

## See Also

### Notifications

class let didChangeNotification: NSNotification.Name

Posted when user defaults are changed within the current process.

class let sizeLimitExceededNotification: NSNotification.Name

Posted when more data is stored in user defaults than is allowed.

class let completedInitialCloudSyncNotification: NSNotification.Name

Posted when ubiquitous defaults finish downloading data, either the first time a device is connected to an iCloud account or when a user switches their primary iCloud account.

class let didChangeCloudAccountsNotification: NSNotification.Name

Posted when the user changes the primary iCloud account.

