

- Core Data
- NSMergeConflict
-  newVersionNumber 

Instance Property

# newVersionNumber

The new version number for the change.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var newVersionNumber: Int { get }
```

## Discussion

A new version number of 0 means the object was deleted and the corresponding snapshot is `nil`.

## See Also

### Accessing Merge Conflict Details

var sourceObject: NSManagedObject

The source object for the conflict.

var objectSnapshot: [String : Any]?

A dictionary containing the values of the source object.

var cachedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store coordinator layer.

var persistedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store.

var oldVersionNumber: Int

The old version number for the change.

