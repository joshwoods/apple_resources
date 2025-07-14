

- Hypervisor
-  hv_vm_config_get_el2_supported(\_:) 

Function

# hv_vm_config_get_el2_supported(\_:)

Returns a status value that indicates whether the current platform supports Exception Level 2 (EL2).

macOS 15.0+

``` source
func hv_vm_config_get_el2_supported(_ el2_supported: UnsafeMutablePointer) -> hv_return_t
```

## Parameters 

`el2_supported`  

A pointer to a Boolean value that indicates whether the current platform supports EL2. The framework writes this value on success; otherwise, `nil`.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Nested virtualization

func hv_vm_config_get_el2_enabled(hv_vm_config_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Return a status value that indicates whether the VM configuration enables support for Exception Level 2 (EL2).

func hv_vm_config_set_el2_enabled(hv_vm_config_t, Bool) -> hv_return_t

Sets whether the specified VM configuration enables support for Exception Level 2 (EL2).

