

- GSS
-  GSS_IOV_BUFFER_FLAG_ALLOCATED 

Global Variable

# GSS_IOV_BUFFER_FLAG_ALLOCATED

The caller should free the buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var GSS_IOV_BUFFER_FLAG_ALLOCATED: Int32 { get }
```

## See Also

### Buffer Flags

var GSS_IOV_BUFFER_FLAG_ALLOCATE: Int32

GSS should perform the allocation.

var GSS_IOV_BUFFER_TYPE_DATA: Int32

The buffer type is packet data.

var GSS_IOV_BUFFER_TYPE_EMPTY: Int32

The buffer type is empty.

var GSS_IOV_BUFFER_TYPE_FLAG_ALLOCATE: Int32

GSS should perform the allocation.

var GSS_IOV_BUFFER_TYPE_FLAG_ALLOCATED: Int32

The caller should free the buffer.

var GSS_IOV_BUFFER_TYPE_FLAG_MASK: UInt32

The buffer type is a flag mask.

var GSS_IOV_BUFFER_TYPE_HEADER: Int32

The buffer type is a mechanism header.

var GSS_IOV_BUFFER_TYPE_MECH_PARAMS: Int32

The buffer contains mechanism-specific parameters.

var GSS_IOV_BUFFER_TYPE_PADDING: Int32

The buffer contains padding.

var GSS_IOV_BUFFER_TYPE_SIGN_ONLY: Int32

The buffer contains sign-only packet data.

var GSS_IOV_BUFFER_TYPE_STREAM: Int32

The buffer contains a complete wrap token.

var GSS_IOV_BUFFER_TYPE_TRAILER: Int32

The buffer contains a mechanism trailer.

