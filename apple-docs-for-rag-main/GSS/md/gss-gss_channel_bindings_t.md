

- GSS
-  gss_channel_bindings_t 

Type Alias

# gss_channel_bindings_t

A pointer to a channel bindings descriptor that specifies the communications channel used to carry a context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
typealias gss_channel_bindings_t = UnsafeMutablePointer
```

## Topics

### Instance Properties

var acceptor_address: gss_buffer_desc

The network address of the acceptor, in the form specified by acceptor_addrtype.

var acceptor_addrtype: OM_uint32

The type of address contained in the acceptor_address field.

var application_data: gss_buffer_desc

Application specific data for use in communicating a channel binding.

var initiator_address: gss_buffer_desc

The network address of the acceptor, in the form specified by initiator_addrtype.

var initiator_addrtype: OM_uint32

The type of address contained in the initiator_address field.

## See Also

### Channel Bindings

typealias gss_ctx_id_t

A pointer to an opaque type that you use to communicate context pointers with GSS-API functions.

struct gss_channel_bindings_struct

The structure defining a channel bindings descriptor that specifies the communications channel used to carry a context.

typealias gss_const_channel_bindings_t

A pointer to an immutable channel bindings descriptor that you use to specify the communications channel used to carry a context.

