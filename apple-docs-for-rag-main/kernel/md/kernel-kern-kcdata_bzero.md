

- Kernel
- kern
-  kcdata_bzero 

Function

# kcdata_bzero

macOS 10.14+

``` source
kern_return_t kcdata_bzero(kcdata_descriptor_t data, mach_vm_address_t dst_addr, uint32_t size);
```

## See Also

### C Data

kcdata_calc_padding

kcdata_estimate_required_buffer_size

kcdata_flags_get_padding

kcdata_get_memory_addr

kcdata_get_memory_addr_for_array

kcdata_iter

kcdata_iter_array_elem_count

kcdata_iter_array_elem_size

kcdata_iter_array_elem_type

kcdata_iter_array_size_switch

kcdata_iter_array_valid

kcdata_iter_container_id

kcdata_iter_container_type

kcdata_iter_container_valid

kcdata_iter_data_with_desc_valid

kcdata_iter_find_type

kcdata_iter_flags

kcdata_iter_get_data_with_desc

kcdata_iter_is_legacy_item

kcdata_iter_next

kcdata_iter_payload

kcdata_iter_size

kcdata_iter_string

kcdata_iter_type

kcdata_iter_valid

kcdata_memcpy

kcdata_memory_get_used_bytes

