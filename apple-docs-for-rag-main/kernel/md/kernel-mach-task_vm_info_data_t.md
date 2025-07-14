

- Kernel
- mach
-  task_vm_info_data_t 

Structure

# task_vm_info_data_t

macOS 10.9+

``` source
typedef struct task_vm_info {
    ...
} task_vm_info_data_t;
```

## Topics

### Instance Properties

compressed

compressed_lifetime

compressed_peak

decompressions

device

device_peak

external

external_peak

internal

internal_peak

ledger_phys_footprint_peak

ledger_purgeable_nonvolatile

ledger_purgeable_novolatile_compressed

ledger_purgeable_volatile

ledger_purgeable_volatile_compressed

ledger_swapins

ledger_tag_graphics_footprint

ledger_tag_graphics_footprint_compressed

ledger_tag_graphics_nofootprint

ledger_tag_graphics_nofootprint_compressed

ledger_tag_media_footprint

ledger_tag_media_footprint_compressed

ledger_tag_media_nofootprint

ledger_tag_media_nofootprint_compressed

ledger_tag_network_nonvolatile

ledger_tag_network_nonvolatile_compressed

ledger_tag_network_volatile

ledger_tag_network_volatile_compressed

ledger_tag_neural_footprint

ledger_tag_neural_footprint_compressed

ledger_tag_neural_nofootprint

ledger_tag_neural_nofootprint_compressed

ledger_tag_neural_nofootprint_peak

ledger_tag_neural_nofootprint_total

limit_bytes_remaining

max_address

min_address

page_size

phys_footprint

purgeable_volatile_pmap

purgeable_volatile_resident

purgeable_volatile_virtual

region_count

resident_size

resident_size_peak

reusable

reusable_peak

virtual_size

## See Also

### Task

mach_task_flavor_t

task_absolutetime_info_t

task_access_subsystem

task_affinity_tag_info_t

task_array_t

task_basic_info_32_t

task_basic_info_64_t

task_basic_info_t

task_category_policy_t

task_delta_snapshot_v2

task_dyld_info_t

task_events_info_t

task_exc_guard_behavior_t

task_extmod_info_t

task_flags_info_t

task_flavor_t

task_info_data_t

task_info_t

task_inspect_basic_counts_t

task_inspect_flavor

task_inspect_flavor_t

task_inspect_info_t

task_inspect_t

task_kernelmemory_info_t

task_latency_qos

task_latency_qos_t

task_name_t

task_policy_flavor_t

task_policy_t

task_port_array_t

task_port_t

task_power_info_t

task_power_info_v2_t

task_purgable_info_t

task_restartable_range_array_t

task_snapshot

task_snapshot_flags

task_snapshot_v2

task_special_port_t

task_suspension_token_t

task_t

task_thread_times_info_t

task_throughput_qos

task_throughput_qos_t

task_trace_memory_info_t

task_vm_info_t

task_wait_state_info_t

task_zone_info_array_t

mach_task_basic_info_t

mach_task_basic_info_data_t

task_absolutetime_info_data_t

task_affinity_tag_info_data_t

task_basic_info_32_data_t

task_basic_info_64_data_t

task_basic_info_data_t

task_category_policy_data_t

task_crashinfo_item_t

task_dyld_info_data_t

task_events_info_data_t

task_extmod_info_data_t

task_flags_info_data_t

task_gate_t

task_inspect_basic_counts_data_t

task_kernelmemory_info_data_t

task_power_info_data_t

task_power_info_v2_data_t

task_qos_policy_t

task_restartable_range_t

task_thread_times_info_data_t

task_trace_memory_info_data_t

task_wait_state_info_data_t

task_zone_info_t

check_task_access

