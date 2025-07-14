

- Core Data
- NSMigrationManager
-  usesStoreSpecificMigrationManager 

Instance Property

# usesStoreSpecificMigrationManager

A Boolean value that indicates whether the migration manager tries to use a store specific migration manager to perform the migration.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var usesStoreSpecificMigrationManager: Bool { get set }
```

## Return Value

true if the receiver uses a store-specific migration manager, otherwise false.

## Discussion

true if the receiver uses a store-specific migration manager, otherwise false. The default value is true.

A store-specific migration manager class is not guaranteed to perform any of the migration manager delegate callbacks or update values for the observable properties.

## See Also

### Customizing the Manager

var userInfo: [AnyHashable : Any]?

The user info for the migration manager.

