

- Core Data
- NSPersistentStoreDescription
-  sqlitePragmas 

Instance Property

# sqlitePragmas

The SQLite pragmas set for the associated persistent store. (read-only)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var sqlitePragmas: [String : NSObject] { get }
```

## Discussion

This property contains all of the pragmas set on the associated persistent store. This property is only relevant when the type is set to NSSQLiteStoreType.

## See Also

### Accessing the Configuration Options

var options: [String : NSObject]

A dictionary representation of the options set on the associated persistent store.

