

- GSS
- gss_channel_bindings_struct
-  application_data 

Instance Property

# application_data

Application specific data for use in communicating a channel binding.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var application_data: gss_buffer_desc
```

## See Also

### Instance Properties

var initiator_addrtype: OM_uint32

The type of address contained in the initiator_address field.

var initiator_address: gss_buffer_desc

The network address of the acceptor, in the form specified by initiator_addrtype.

var acceptor_addrtype: OM_uint32

The type of address contained in the acceptor_address field.

var acceptor_address: gss_buffer_desc

The network address of the acceptor, in the form specified by acceptor_addrtype.

