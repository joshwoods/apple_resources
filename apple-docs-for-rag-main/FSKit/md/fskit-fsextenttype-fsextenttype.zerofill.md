

- FSKit
- FSExtentType
-  FSExtentType.zeroFill 

Case

# FSExtentType.zeroFill

An extent type to indicate uninitialized data.

macOS 15.4+

``` source
case zeroFill
```

## Discussion

Only use this extent type in file systems that support sparse files, and only then to represent ranges in the file that aren’t allocated yet.

## See Also

### Working with extent types

case data

An extent type to indicate valid data.

