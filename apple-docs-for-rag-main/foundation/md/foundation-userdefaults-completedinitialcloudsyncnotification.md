

- Foundation
- UserDefaults
-  completedInitialCloudSyncNotification 

Type Property

# completedInitialCloudSyncNotification

Posted when ubiquitous defaults finish downloading data, either the first time a device is connected to an iCloud account or when a user switches their primary iCloud account.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let completedInitialCloudSyncNotification: NSNotification.Name
```

## Discussion

This notification is posted on the main queue.

## See Also

### Notifications

class let didChangeNotification: NSNotification.Name

Posted when user defaults are changed within the current process.

class let sizeLimitExceededNotification: NSNotification.Name

Posted when more data is stored in user defaults than is allowed.

class let didChangeCloudAccountsNotification: NSNotification.Name

Posted when the user changes the primary iCloud account.

class let noCloudAccountNotification: NSNotification.Name

Posted when a cloud default is set, but no iCloud user is logged in.

