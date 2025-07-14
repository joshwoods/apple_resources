

- FSKit
- FSError
- FSError.Code
-  FSError.Code.resourceUnrecognized 

Case

# FSError.Code.resourceUnrecognized

FSKit didn’t recognize the resource, and probing failed to find a match.

macOS 15.4+

``` source
case resourceUnrecognized
```

## See Also

### Identifying errors

case invalidDirectoryCookie

While enumerating a directory, the given cookie didn’t resolve to a valid directory entry.

case moduleLoadFailed

The module failed to load.

case resourceDamaged

The resource is damaged.

case resourceUnusable

FSKit recognizes the resource, but the resource isn’t usable.

case statusOperationInProgress

An operation is in progress.

case statusOperationPaused

An operation is paused.

