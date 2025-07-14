

- FSKit
- FSExtentType
-  FSExtentType.data 

Case

# FSExtentType.data

An extent type to indicate valid data.

macOS 15.4+

``` source
case data
```

## Discussion

Use this type for all extents on a file system that doesn’t support sparse files.

Tip

The kernel keeps track of the end of file, so it knows a range of `[EOF, allocated space]` is uninitialized. Because of this behavior, it’s valid to pass the data extent type for such a range.

## See Also

### Working with extent types

case zeroFill

An extent type to indicate uninitialized data.

