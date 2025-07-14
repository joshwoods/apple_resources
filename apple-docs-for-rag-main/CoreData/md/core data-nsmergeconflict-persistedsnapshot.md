

- Core Data
- NSMergeConflict
-  persistedSnapshot 

Instance Property

# persistedSnapshot

A dictionary containing the values of the source object held in the persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var persistedSnapshot: [String : Any]? { get }
```

## See Also

### Accessing Merge Conflict Details

var sourceObject: NSManagedObject

The source object for the conflict.

var objectSnapshot: [String : Any]?

A dictionary containing the values of the source object.

var cachedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store coordinator layer.

var newVersionNumber: Int

The new version number for the change.

var oldVersionNumber: Int

The old version number for the change.

