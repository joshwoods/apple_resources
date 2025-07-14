

- Foundation
- UserDefaults
-  didChangeNotification 

Type Property

# didChangeNotification

Posted when user defaults are changed within the current process.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let didChangeNotification: NSNotification.Name
```

## Discussion

This notification is posted on the thread that changes the user defaults. The notification object is the UserDefaults object. The notification doesn’t contain a userInfo dictionary.

This notification isn’t posted when changes are made outside the current process, or when ubiquitous defaults change. You can use key-value observing to register observers for specific keys of interest in order to be notified of all updates, regardless of whether changes are made within or outside the current process.

## See Also

### Notifications

class let sizeLimitExceededNotification: NSNotification.Name

Posted when more data is stored in user defaults than is allowed.

class let completedInitialCloudSyncNotification: NSNotification.Name

Posted when ubiquitous defaults finish downloading data, either the first time a device is connected to an iCloud account or when a user switches their primary iCloud account.

class let didChangeCloudAccountsNotification: NSNotification.Name

Posted when the user changes the primary iCloud account.

class let noCloudAccountNotification: NSNotification.Name

Posted when a cloud default is set, but no iCloud user is logged in.

