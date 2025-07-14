

- FSKit
- FSError
- FSError.Code
-  FSError.Code.invalidDirectoryCookie 

Case

# FSError.Code.invalidDirectoryCookie

While enumerating a directory, the given cookie didn’t resolve to a valid directory entry.

macOS 15.4+

``` source
case invalidDirectoryCookie
```

## See Also

### Identifying errors

case moduleLoadFailed

The module failed to load.

case resourceDamaged

The resource is damaged.

case resourceUnrecognized

FSKit didn’t recognize the resource, and probing failed to find a match.

case resourceUnusable

FSKit recognizes the resource, but the resource isn’t usable.

case statusOperationInProgress

An operation is in progress.

case statusOperationPaused

An operation is paused.

