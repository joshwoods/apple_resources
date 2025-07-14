

- GSS
-  Buffer Management 

API Collection

# Buffer Management

Allocate and deallocate buffers with structures that hold a variety of data.

## Topics

### Buffer Data Structures

typealias gss_qop_t

A quality of protection setting.

typealias gss_iov_buffer_t

The structure for a vectored I/O buffer and its defined type.

typealias gss_iov_buffer_desc

The structure for a vectored I/O buffer and its defined type.

struct gss_iov_buffer_desc_struct

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

### Allocation and Deallocation

func gss_create_empty_buffer_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Allocates an empty buffer set descriptor that you use to manage an array of buffers.

func gss_add_buffer_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_buffer_set_t>) -> OM_uint32

Copies the contents of a buffer into a buffer set.

func gss_release_buffer(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t) -> OM_uint32

Frees the memory associated with a single buffer descriptor.

func gss_release_buffer_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Frees the memory associated with a buffer set descriptor and all the buffers it contains.

## See Also

### Memory and Context

Allocating and Releasing Objects

Manage memory and object lifetimes.

Function Status

Evaluate return values that most GSS-API functions use to indicate the outcome of an operation.

Context Services

Use context services to manage secure operations between endpoints.

