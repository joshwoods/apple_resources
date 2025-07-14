

- Endpoint Security
- es_file_t
-  stat 

Instance Property

# stat

The file’s metadata, such as file size, user and group identifiers, and access and modification dates.

Mac CatalystmacOS

``` source
var stat: stat
```

## Discussion

The returned structure’s information is equivalent to that returned by the `stat(2)` system call.

## See Also

### Inspecting File Properties

var path: es_string_token_t

The file’s path.

var path_truncated: Bool

A Boolean value that indicates whether Endpoint Security truncated the path string.

