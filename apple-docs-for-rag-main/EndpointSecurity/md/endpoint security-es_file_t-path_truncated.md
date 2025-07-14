

- Endpoint Security
- es_file_t
-  path_truncated 

Instance Property

# path_truncated

A Boolean value that indicates whether Endpoint Security truncated the path string.

Mac CatalystmacOS

``` source
var path_truncated: Bool
```

## Discussion

If Endpoint Security truncated the full file path when assigning the path field, this value is `true`.

## See Also

### Inspecting File Properties

var path: es_string_token_t

The file’s path.

var stat: stat

The file’s metadata, such as file size, user and group identifiers, and access and modification dates.

