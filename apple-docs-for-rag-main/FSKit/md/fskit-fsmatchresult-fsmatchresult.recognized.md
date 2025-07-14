

- FSKit
- FSMatchResult
-  FSMatchResult.recognized 

Case

# FSMatchResult.recognized

The probe recognizes the resource but can’t use it.

macOS 15.4+

``` source
case recognized
```

## Discussion

This match result is appropriate when the file system module identifies the resource’s format but can’t use it. For example, if the resource uses a newer version than the module supports, the module can name the resource but can’t safely do anything with it.

## See Also

### Working with match results

case usable

The probe recognizes the resource and is ready to use it.

case usableButLimited

The probe recognizes the resource and is ready to use it, but only in a limited capacity.

case notRecognized

The probe doesn’t recognize the resource.

