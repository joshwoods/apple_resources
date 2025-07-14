

- Core Data
- NSMergeConflict
-  init(source:newVersion:oldVersion:cachedSnapshot:persistedSnapshot:) 

Initializer

# init(source:newVersion:oldVersion:cachedSnapshot:persistedSnapshot:)

Initializes a merge conflict.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    source srcObject: NSManagedObject,
    newVersion newvers: Int,
    oldVersion oldvers: Int,
    cachedSnapshot cachesnap: [String : Any]?,
    persistedSnapshot persnap: [String : Any]?
)
```

## Parameters 

`srcObject`  

The source object for the conflict.

`newvers`  

The new version number for the change.

A value of 0 means the object was deleted and the corresponding snapshot is `nil`.

`oldvers`  

The old version number for the change.

`cachesnap`  

A dictionary containing the values of `srcObject` held in the persistent store coordinator layer.

`persnap`  

A dictionary containing the values of `srcObject` held in the persistent store.

## Return Value

A merge conflict object initialized with the given parameters.

## See Also

### Related Documentation

Core Data Model Versioning and Data Migration Programming Guide

