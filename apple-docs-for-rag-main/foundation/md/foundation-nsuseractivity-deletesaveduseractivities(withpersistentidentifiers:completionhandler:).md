

- Foundation
- NSUserActivity
-  deleteSavedUserActivities(withPersistentIdentifiers:completionHandler:) 

Type Method

# deleteSavedUserActivities(withPersistentIdentifiers:completionHandler:)

Deletes user activities created by your app that have the specified persistent identifiers.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 5.0+

``` source
class func deleteSavedUserActivities(
    withPersistentIdentifiers persistentIdentifiers: [NSUserActivityPersistentIdentifier],
    completionHandler handler: @escaping () -> Void
)
```

``` source
class func deleteSavedUserActivities(withPersistentIdentifiers persistentIdentifiers: [NSUserActivityPersistentIdentifier]) async
```

## Parameters 

`persistentIdentifiers`  

The list of persistent identifiers that the system uses to determine which user activities to delete.

`handler`  

The block that the system invokes after deleting the user activities. Wait for the system to call this block to ensure that the system deletes the activities (or marks them for deletion).

## Discussion

Deletes user activities with a persistent identifier matching any identifier in the `persistentIdentifiers` array.

## See Also

### Deleting saved user activities

class func deleteAllSavedUserActivities(completionHandler: () -> Void)

Deletes all user activities created by your app.

