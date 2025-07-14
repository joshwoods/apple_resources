

- Core Data
- NSMergeConflict
-  objectSnapshot 

Instance Property

# objectSnapshot

A dictionary containing the values of the source object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var objectSnapshot: [String : Any]? { get }
```

## See Also

### Accessing Merge Conflict Details

var sourceObject: NSManagedObject

The source object for the conflict.

var cachedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store coordinator layer.

var persistedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store.

var newVersionNumber: Int

The new version number for the change.

var oldVersionNumber: Int

The old version number for the change.

