

- FSKit
- FSError
- FSError.Code
-  FSError.Code.resourceUnusable 

Case

# FSError.Code.resourceUnusable

FSKit recognizes the resource, but the resource isn’t usable.

macOS 15.4+

``` source
case resourceUnusable
```

## Discussion

For example, this error occurs when a resource uses a file system’s internal feature flags. If the only modules that support the file system don’t support those feature flags, this code indicates an unusable resource. The error tells the person using the module why the resource isn’t usable.

## See Also

### Identifying errors

case invalidDirectoryCookie

While enumerating a directory, the given cookie didn’t resolve to a valid directory entry.

case moduleLoadFailed

The module failed to load.

case resourceDamaged

The resource is damaged.

case resourceUnrecognized

FSKit didn’t recognize the resource, and probing failed to find a match.

case statusOperationInProgress

An operation is in progress.

case statusOperationPaused

An operation is paused.

