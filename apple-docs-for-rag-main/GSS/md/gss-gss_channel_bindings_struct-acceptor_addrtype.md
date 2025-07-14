

- GSS
- gss_channel_bindings_struct
-  acceptor_addrtype 

Instance Property

# acceptor_addrtype

The type of address contained in the acceptor_address field.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var acceptor_addrtype: OM_uint32
```

## Discussion

The field takes one of the constants listed in `Address Families`.

## See Also

### Instance Properties

var initiator_addrtype: OM_uint32

The type of address contained in the initiator_address field.

var initiator_address: gss_buffer_desc

The network address of the acceptor, in the form specified by initiator_addrtype.

var acceptor_address: gss_buffer_desc

The network address of the acceptor, in the form specified by acceptor_addrtype.

var application_data: gss_buffer_desc

Application specific data for use in communicating a channel binding.

