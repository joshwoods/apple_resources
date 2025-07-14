

- Endpoint Security
- es_fd_t
-  fdtype 

Instance Property

# fdtype

The file descriptor type, as a libproc type.

Mac CatalystmacOS

``` source
var fdtype: UInt32
```

## Discussion

If this value is `PROX_FDTYPE_PIPE`, the es_fd_t structure also contains a `pipe.pipe_id` field. This field represents the unique ID of the pipe for correlation with other file descriptors pointing to the same or other end of the same pipe.

## See Also

### Inspecting File Descriptor Properties

var fd: Int32

The file descriptor number.

