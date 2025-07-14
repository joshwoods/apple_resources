

- Kernel
- mach
-  thread_set_thread_name 

Function

# thread_set_thread_name

macOS 10.15+

``` source
void thread_set_thread_name(thread_t th, const char *name);
```

## See Also

### Thread

current_thread

thread_abort

thread_abort_safely

thread_assign

thread_assign_default

thread_block

thread_block_parameter

thread_call_allocate

Allocate a thread call to execute with default (high) priority.

thread_call_allocate_with_options

thread_call_allocate_with_priority

Allocate a thread call to execute with a specified priority.

thread_call_cancel

Attempt to cancel a pending invocation of a thread call.

thread_call_cancel_wait

Attempt to cancel a pending invocation of a thread call. If unable to cancel, wait for current invocation to finish.

thread_call_enter

Submit a thread call work item for immediate execution.

thread_call_enter1

Submit a thread call work item for immediate execution, with an extra parameter.

thread_call_enter1_delayed

Submit a thread call to be executed at some point in the future, with an extra parameter.

thread_call_enter_delayed

Submit a thread call to be executed at some point in the future.

thread_call_free

Release a thread call.

thread_call_isactive

Determine whether a thread call is pending or currently executing.

thread_create

thread_create_running

thread_deallocate

thread_depress_abort

thread_get_assignment

thread_get_exception_ports

thread_get_mach_voucher

thread_get_special_port

thread_get_state

thread_has_thread_name

thread_info

thread_policy

thread_policy_get

thread_policy_set

thread_reference

thread_resume

thread_sample

thread_set_exception_ports

thread_set_mach_voucher

thread_set_policy

thread_set_special_port

thread_set_state

thread_suspend

thread_swap_exception_ports

thread_swap_mach_voucher

thread_terminate

thread_tid

thread_wakeup_prim

thread_wakeup_thread

thread_wire

thread_act_array_t

thread_act_port_array_t

thread_act_port_t

thread_act_t

thread_affinity_policy_t

thread_array_t

thread_background_policy_t

thread_basic_info_t

thread_call_func_t

thread_call_options_t

thread_call_param_t

thread_call_t

thread_command

thread_continue_t

thread_delta_snapshot_v2

thread_delta_snapshot_v3

thread_extended_info_t

thread_extended_policy_t

thread_flavor_t

mach_thread_flavor_t

thread_group_flags

thread_group_snapshot

thread_group_snapshot_v2

thread_identifier_info_t

thread_info_data_t

thread_info_t

thread_inspect_t

thread_latency_qos_policy_t

thread_latency_qos_t

thread_policy_flavor_t

thread_policy_t

thread_port_array_t

thread_port_t

thread_precedence_policy_t

thread_snapshot

thread_snapshot_flags

thread_snapshot_v2

thread_snapshot_v3

thread_snapshot_v4

thread_standard_policy_t

thread_state_data_t

thread_state_flavor_array_t

thread_state_flavor_t

thread_state_t

thread_t

thread_throughput_qos_policy_t

thread_throughput_qos_t

thread_time_constraint_policy_t

thread_affinity_policy_data_t

thread_background_policy_data_t

thread_basic_info_data_t

thread_extended_info_data_t

thread_extended_policy_data_t

thread_identifier_info_data_t

thread_latency_qos_policy_data_t

thread_precedence_policy_data_t

thread_standard_policy_data_t

thread_throughput_qos_policy_data_t

thread_time_constraint_policy_data_t

thread_turnstileinfo_t

thread_waitinfo_t

act_get_state

act_set_state

