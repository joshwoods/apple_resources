

- Kernel
- mach
-  vm 

API Collection

# vm

Create, destroy, and access pages in the virtual memory system.

## Topics

### Creation and Destruction

vm_allocate

vm_allocate_cpm

vm_deallocate

vm_copy

mach_vm_copy

### Memory Mapping

vm_map

vm_map_64

vm_map_exec_lockdown

vm_map_page_query

vm_mapped_pages_info

vm_remap

mach_make_memory_entry

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

### Reads and Writes

vm_read

vm_read_list

vm_read_overwrite

vm_write

### Configuration

vm_protect

vm_wire

mach_memory_info

vm_behavior_set

vm_machine_attribute

vm_purgable_control

vm_inherit

vm_msync

### Regions

vm_region

vm_region_64

vm_region_recurse

vm_region_recurse_64

vm_region_basic_info_data_64_t

vm_region_basic_info_data_t

vm_region_extended_info_data_t

vm_region_submap_info_data_64_t

vm_region_submap_info_data_t

vm_region_submap_short_info_data_64_t

vm_region_top_info_data_t

vm_page_info_basic_data_t

### VM Types

vm_read_entry_t

vm_map_inspect_t

vm_map_read_t

vm_address_t

vm_behavior_t

vm_extmod_statistics_t

vm_info_object_array_t

vm_inherit_t

vm_machine_attribute_t

vm_machine_attribute_val_t

vm_map_address_t

vm_map_offset_t

vm_map_size_t

vm_map_t

vm_named_entry_t

vm_object_id_t

vm_object_offset_t

vm_object_size_t

vm_offset_t

vm_page_info_basic_t

vm_page_info_data_t

vm_page_info_flavor_t

vm_page_info_t

vm_prot_t

vm_purgable_t

vm_purgeable_info_t

vm_region_basic_info_64_t

vm_region_basic_info_t

vm_region_extended_info_t

vm_region_flavor_t

vm_region_info_64_t

vm_region_info_data_t

vm_region_info_t

vm_region_recurse_info_64_t

vm_region_recurse_info_t

vm_region_submap_info_64_t

vm_region_submap_info_t

vm_region_submap_short_info_64_t

vm_region_top_info_t

vm_size_t

vm_statistics64_t

vm_statistics_t

vm_sync_t

vm_task_entry_t

vm32_object_id_t

vm32_address_t

vm32_offset_t

vm32_size_t

### Memory Objects

mach_memory_object_memory_entry

mach_memory_object_memory_entry_64

### Memory Object Types

memory_object_array_t

memory_object_attr_info_t

memory_object_behave_info_t

memory_object_cluster_size_t

memory_object_control_t

memory_object_copy_strategy_t

memory_object_default_t

memory_object_fault_info_t

memory_object_flavor_t

memory_object_info_data_t

memory_object_info_t

memory_object_name_t

memory_object_offset_t

memory_object_perf_info_t

memory_object_return_t

memory_object_size_t

memory_object_t

### Debug

vm_info_region_64_t

vm_info_region_t

vm_info_object_t

### Statistics

vm_statistics64_data_t

vm_statistics_data_t

vm_extmod_statistics_data_t

vm_purgeable_stat_t

## See Also

### Memory

Mach VM

