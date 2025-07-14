

- Foundation
- UserDefaults
-  sizeLimitExceededNotification 

Type Property

# sizeLimitExceededNotification

Posted when more data is stored in user defaults than is allowed.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let sizeLimitExceededNotification: NSNotification.Name
```

## Discussion

This notification is posted on the main queue.

Currently, there is only a size limit for data stored to local user defaults on tvOS, which posts a warning notification when user defaults storage reaches 512kB in size, and terminates apps when user defaults storage reaches 1MB in size.

For ubiquitous defaults, the limit depends on the logged in iCloud user.

## See Also

### Notifications

class let didChangeNotification: NSNotification.Name

Posted when user defaults are changed within the current process.

class let completedInitialCloudSyncNotification: NSNotification.Name

Posted when ubiquitous defaults finish downloading data, either the first time a device is connected to an iCloud account or when a user switches their primary iCloud account.

class let didChangeCloudAccountsNotification: NSNotification.Name

Posted when the user changes the primary iCloud account.

class let noCloudAccountNotification: NSNotification.Name

Posted when a cloud default is set, but no iCloud user is logged in.

