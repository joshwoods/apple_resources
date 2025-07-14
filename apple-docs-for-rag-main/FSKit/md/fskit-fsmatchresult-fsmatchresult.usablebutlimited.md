

- FSKit
- FSMatchResult
-  FSMatchResult.usableButLimited 

Case

# FSMatchResult.usableButLimited

The probe recognizes the resource and is ready to use it, but only in a limited capacity.

macOS 15.4+

``` source
case usableButLimited
```

## Discussion

This match result is appropriate when the file system module identifies the resource’s format but also identifies incompatibilities. For example, if the module determines the resource uses new features that the module doesn’t support, the module may only offer read-only access.

## See Also

### Working with match results

case usable

The probe recognizes the resource and is ready to use it.

case recognized

The probe recognizes the resource but can’t use it.

case notRecognized

The probe doesn’t recognize the resource.

