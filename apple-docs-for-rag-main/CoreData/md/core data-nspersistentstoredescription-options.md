

- Core Data
- NSPersistentStoreDescription
-  options 

Instance Property

# options

A dictionary representation of the options set on the associated persistent store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var options: [String : NSObject] { get }
```

## Discussion

A dictionary containing key-value pairs that specify numerous settings for the persistent store. For key definitions, see NSPersistentStoreCoordinator.

## See Also

### Accessing the Configuration Options

var sqlitePragmas: [String : NSObject]

The SQLite pragmas set for the associated persistent store. (read-only)

