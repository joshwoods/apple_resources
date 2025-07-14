

- vmnet
-  vmnet_interface_get_port_forwarding_rules(\_:\_:) 

Function

# vmnet_interface_get_port_forwarding_rules(\_:\_:)

Mac Catalyst 13.0+macOS 10.15–12.0Deprecated

``` source
func vmnet_interface_get_port_forwarding_rules(
    _ interface: interface_ref,
    _ handler: @escaping vmnet_interface_get_port_forwarding_rules_handler_t
) -> vmnet_return_t
```

## See Also

### Functions

func vmnet_copy_shared_interface_list() -> xpc_object_t?

func vmnet_interface_add_ip_port_forwarding_rule(interface_ref, UInt8, UInt16, UInt8, UnsafeRawPointer, UInt16, vmnet_interface_completion_handler_t?) -> vmnet_return_t

func vmnet_interface_add_port_forwarding_rule(interface_ref, UInt8, UInt16, in_addr, UInt16, vmnet_interface_completion_handler_t?) -> vmnet_return_t

func vmnet_interface_get_ip_port_forwarding_rules(interface_ref, UInt8, vmnet_interface_get_ip_port_forwarding_rules_handler_t) -> vmnet_return_t

func vmnet_interface_remove_ip_port_forwarding_rule(interface_ref, UInt8, UInt16, UInt8, vmnet_interface_completion_handler_t?) -> vmnet_return_t

func vmnet_interface_remove_port_forwarding_rule(interface_ref, UInt8, UInt16, vmnet_interface_completion_handler_t?) -> vmnet_return_t

func vmnet_ip_port_forwarding_rule_get_details(xpc_object_t, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;UInt16>, UInt8, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt16>) -> vmnet_return_t

func vmnet_port_forwarding_rule_get_details(xpc_object_t, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;UInt16>, UnsafeMutablePointer&lt;in_addr>, UnsafeMutablePointer&lt;UInt16>) -> vmnet_return_t

