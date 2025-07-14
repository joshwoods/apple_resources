

- GSS
-  gss_iov_buffer_desc_struct 

Structure

# gss_iov_buffer_desc_struct

The structure for a vectored I/O buffer and its defined type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
struct gss_iov_buffer_desc_struct
```

## Topics

### Instance Properties

var buffer: gss_buffer_desc

The buffer length and contents.

var type: OM_uint32

The buffer type.

### Initialization

init()

Initialize a new, empty IOV buffer structure.

init(type: OM_uint32, buffer: gss_buffer_desc)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Buffer Data Structures

typealias gss_qop_t

A quality of protection setting.

typealias gss_iov_buffer_t

The structure for a vectored I/O buffer and its defined type.

typealias gss_iov_buffer_desc

The structure for a vectored I/O buffer and its defined type.

typealias gss_buffer_t

A pointer to a buffer descriptor that you use to exchange octet streams with many GSS-API functions.

typealias gss_const_buffer_t

A pointer to an immutable buffer descriptor that you use to exchange octet streams with many GSS-API functions.

typealias gss_buffer_set_t

A pointer to the descriptor that you use to manage an array of buffer descriptors.

typealias gss_buffer_desc

The buffer descriptor that you use to exchange octet streams with many GSS-API functions.

struct gss_buffer_desc_struct

The structure for a buffer descriptor that you use to exchange octet streams with many GSS-API functions.

typealias gss_buffer_set_desc

The descriptor that you use to manage an array of buffer descriptors.

struct gss_buffer_set_desc_struct

The structure for a buffer set descriptor that you use to manage an array of buffer descriptors.

