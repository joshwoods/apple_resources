

- FSKit
- FSMatchResult
-  FSMatchResult.notRecognized 

Case

# FSMatchResult.notRecognized

The probe doesn’t recognize the resource.

macOS 15.4+

``` source
case notRecognized
```

## Discussion

This match result is appropriate when the file system module determines that the resource uses a completely different format.

## See Also

### Working with match results

case usable

The probe recognizes the resource and is ready to use it.

case usableButLimited

The probe recognizes the resource and is ready to use it, but only in a limited capacity.

case recognized

The probe recognizes the resource but can’t use it.

