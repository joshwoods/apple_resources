

- Kernel
- mach
-  task_snapshot 

# task_snapshot

macOS 10.7+

``` source
struct task_snapshot {
    ...
};
```

## Topics

### Instance Properties

cow_faults

data_count

data_size

did_throttle

disk_reads_count

disk_reads_size

disk_writes_count

disk_writes_size

donating_pid_count

faults

io_priority_count

io_priority_size

latency_qos

metadata_count

metadata_size

nloadinfos

non_paging_count

non_paging_size

p_comm

p_start_sec

p_start_usec

pageins

paging_count

paging_size

pid

shared_cache_identifier

shared_cache_slide

snapshot_magic

ss_flags

suspend_count

system_time_in_terminated_threads

task_size

uniqueid

user_time_in_terminated_threads

was_throttled

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

task_vm_info_data_t

task_wait_state_info_data_t

task_zone_info_t

check_task_access

