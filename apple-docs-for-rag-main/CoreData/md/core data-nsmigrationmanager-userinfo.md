

- Core Data
- NSMigrationManager
-  userInfo 

Instance Property

# userInfo

The user info for the migration manager.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

You can use the user info dictionary to aid the customization of your migration process.

## See Also

### Customizing the Manager

var usesStoreSpecificMigrationManager: Bool

A Boolean value that indicates whether the migration manager tries to use a store specific migration manager to perform the migration.

