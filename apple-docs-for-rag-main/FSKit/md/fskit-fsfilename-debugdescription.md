

- FSKit
- FSFileName
-  debugDescription 

Instance Property

# debugDescription

The filename, represented as a potentially lossy conversion to a string.

macOS 15.4+

``` source
var debugDescription: String { get }
```

## Discussion

The exact details of the string conversion may change in the future.

## See Also

### Accessing filename properties

var data: Data

The byte sequence of the filename, as a data object.

var string: String?

The filename, represented as a Unicode string.

