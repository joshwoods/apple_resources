

- FSKit
- FSError
- FSError.Code
-  FSError.Code.statusOperationInProgress 

Case

# FSError.Code.statusOperationInProgress

An operation is in progress.

macOS 15.4+

``` source
case statusOperationInProgress
```

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

case resourceUnusable

FSKit recognizes the resource, but the resource isn’t usable.

case statusOperationPaused

An operation is paused.

