

- Foundation
- NSUserActivity
-  deleteAllSavedUserActivities(completionHandler:) 

Type Method

# deleteAllSavedUserActivities(completionHandler:)

Deletes all user activities created by your app.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 5.0+

``` source
class func deleteAllSavedUserActivities(completionHandler handler: @escaping () -> Void)
```

``` source
class func deleteAllSavedUserActivities() async
```

## Parameters 

`handler`  

The block that the system invokes after deleting the user activities. Wait for the system to call this block to ensure that the system deletes the activities (or marks them for deletion).

## Discussion

Deletes all user activities stored by Core Spotlight or donated as Siri shortcuts.

## See Also

### Deleting saved user activities

class func deleteSavedUserActivities(withPersistentIdentifiers: [NSUserActivityPersistentIdentifier], completionHandler: () -> Void)

Deletes user activities created by your app that have the specified persistent identifiers.

