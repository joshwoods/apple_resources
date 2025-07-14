

- FSKit
- FSError
- FSError.Code
-  FSError.Code.resourceDamaged 

Case

# FSError.Code.resourceDamaged

The resource is damaged.

macOS 15.4+

``` source
case resourceDamaged
```

## Discussion

This error indicates the resource needs a repair operation, or that a repair operation failed.

Note

The status in this error applies to the resource. A failing repair operation reports a more specific error status.

## See Also

### Identifying errors

case invalidDirectoryCookie

While enumerating a directory, the given cookie didn’t resolve to a valid directory entry.

case moduleLoadFailed

The module failed to load.

case resourceUnrecognized

FSKit didn’t recognize the resource, and probing failed to find a match.

case resourceUnusable

FSKit recognizes the resource, but the resource isn’t usable.

case statusOperationInProgress

An operation is in progress.

case statusOperationPaused

An operation is paused.

