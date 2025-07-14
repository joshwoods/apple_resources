

- Core Data
- NSPersistentStore
-  migrationManagerClass() 

Type Method

# migrationManagerClass()

Returns the migration manager class for this store class.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func migrationManagerClass() -> AnyClass
```

## Return Value

The `NSMigrationManager` class for this store class

## Discussion

In a subclass of `NSPersistentStore`, you can override this to provide a custom migration manager subclass (for example, to take advantage of store-specific functionality to improve migration performance).

