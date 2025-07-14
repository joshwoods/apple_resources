

- FSKit
- FSFileName
-  string 

Instance Property

# string

The filename, represented as a Unicode string.

macOS 15.4+

``` source
var string: String? { get }
```

## Discussion

If the value of the filename’s data is not a valid UTF-8 byte sequence, this property is empty.

## See Also

### Accessing filename properties

var data: Data

The byte sequence of the filename, as a data object.

var debugDescription: String

The filename, represented as a potentially lossy conversion to a string.

