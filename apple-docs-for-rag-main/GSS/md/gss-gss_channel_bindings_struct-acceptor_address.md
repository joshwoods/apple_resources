

- GSS
- gss_channel_bindings_struct
-  acceptor_address 

Instance Property

# acceptor_address

The network address of the acceptor, in the form specified by acceptor_addrtype.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var acceptor_address: gss_buffer_desc
```

## Discussion

If the specified address family has more than one format, the address itself should contain enough information to distinguish among them.

## See Also

### Instance Properties

var initiator_addrtype: OM_uint32

The type of address contained in the initiator_address field.

var initiator_address: gss_buffer_desc

The network address of the acceptor, in the form specified by initiator_addrtype.

var acceptor_addrtype: OM_uint32

The type of address contained in the acceptor_address field.

var application_data: gss_buffer_desc

Application specific data for use in communicating a channel binding.

