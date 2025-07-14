

- Endpoint Security
- es_string_token_t
-  length 

Instance Property

# length

The size of the data buffer, in bytes.

Mac CatalystmacOS

``` source
var length: Int
```

## Discussion

This value doesn’t include the null terminator.

## See Also

### Inspecting the Token

var data: UnsafePointer&lt;CChar>!

The string data.

