

- Endpoint Security
- es_event_close_t
-  modified 

Instance Property

# modified

A Boolean value that indicates whether the file has modifications.

Mac CatalystmacOS

``` source
var modified: Bool
```

## Discussion

This value corresponds to `KAUTH_FILEOP_CLOSE_MODIFIED`.

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_file_t>

The file to close.

