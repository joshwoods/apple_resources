

- GSS
- gss_channel_bindings_struct
-  init(initiator_addrtype:initiator_address:acceptor_addrtype:acceptor_address:application_data:) 

Initializer

# init(initiator_addrtype:initiator_address:acceptor_addrtype:acceptor_address:application_data:)

Initialize a new channel bindings structure with the given configuration.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
init(
    initiator_addrtype: OM_uint32,
    initiator_address: gss_buffer_desc,
    acceptor_addrtype: OM_uint32,
    acceptor_address: gss_buffer_desc,
    application_data: gss_buffer_desc
)
```

## Parameters 

`initiator_addrtype`  

The type of address contained in the `initiator_address` field. Use one of the values found in `Address Families`.

`initiator_address`  

The network address of the initiator, in the form specified by `initiator_addrtype`.

`acceptor_addrtype`  

The type of address contained in the `acceptor_address` field. Use one of the values found in `Address Families`.

`acceptor_address`  

The network address of the acceptor, in the form specified by `acceptor_addrtype`.

`application_data`  

Application specific data for use in communicating a channel binding.

## See Also

### Initialization

init()

Initialize a new, empty channel bindings structure.

