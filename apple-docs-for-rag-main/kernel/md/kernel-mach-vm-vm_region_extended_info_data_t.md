

- Kernel
- mach
- vm
-  vm_region_extended_info_data_t 

Structure

# vm_region_extended_info_data_t

macOS 10.0+

``` source
typedef struct vm_region_extended_info {
    ...
} vm_region_extended_info_data_t;
```

## Topics

### Instance Properties

external_pager

pages_dirtied

pages_resident

pages_reusable

pages_shared_now_private

pages_swapped_out

protection

ref_count

shadow_depth

share_mode

user_tag

## See Also

### Regions

vm_region

vm_region_64

vm_region_recurse

vm_region_recurse_64

vm_region_basic_info_data_64_t

vm_region_basic_info_data_t

vm_region_submap_info_data_64_t

vm_region_submap_info_data_t

vm_region_submap_short_info_data_64_t

vm_region_top_info_data_t

vm_page_info_basic_data_t

