

- Kernel
-  mach 

API Collection

# mach

Access Mach interfaces including processor, memory, thread, and semaphore support.

## Topics

### Memory

vm

Create, destroy, and access pages in the virtual memory system.

Mach VM

### Messages

mach_msg_destroy_from_kernel_proper

mach_msg_overwrite

mach_msg_rpc_from_kernel_proper

mach_msg_send_from_kernel_proper

mach_exc_server

mach_exc_server_routine

audit_triggers_server

audit_triggers_server_routine

mach_msg_audit_trailer_t

mach_msg_base_t

mach_msg_body_t

mach_msg_context_trailer_t

mach_msg_empty_rcv_t

mach_msg_empty_send_t

mach_msg_guarded_port_descriptor32_t

mach_msg_guarded_port_descriptor64_t

mach_msg_guarded_port_descriptor_t

mach_msg_header_t

mach_msg_mac_trailer_t

mach_msg_ool_descriptor32_t

mach_msg_ool_descriptor64_t

mach_msg_ool_descriptor_t

mach_msg_ool_ports_descriptor32_t

mach_msg_ool_ports_descriptor64_t

mach_msg_ool_ports_descriptor_t

mach_msg_port_descriptor_t

mach_msg_security_trailer_t

mach_msg_seqno_trailer_t

mach_msg_trailer_t

mach_msg_type_descriptor_t

mach_msg_bits_t

mach_msg_copy_options_t

mach_msg_descriptor_type_t

mach_msg_format_0_trailer_t

mach_msg_guard_flags_t

mach_msg_id_t

mach_msg_max_trailer_t

mach_msg_option_t

mach_msg_options_t

mach_msg_priority_t

mach_msg_return_t

mach_msg_size_t

mach_msg_timeout_t

mach_msg_trailer_info_t

mach_msg_trailer_size_t

mach_msg_trailer_type_t

mach_msg_type_name_t

mach_msg_type_number_t

mach_msg_type_size_t

mach_msg_filter_id

### MIG

mig_allocate

mig_dealloc_reply_port

mig_deallocate

mig_get_reply_port

mig_put_reply_port

mig_strncpy

mig_strncpy_zerofill

arcade_upcall

arcade_upcall_server

arcade_upcall_server_routine

mig_impl_routine_t

mig_routine_arg_descriptor_t

mig_routine_descriptor_t

mig_routine_t

mig_server_routine_t

mig_stub_routine_t

### Notifications

do_mach_notify_dead_name

do_mach_notify_no_senders

do_mach_notify_port_deleted

do_mach_notify_port_destroyed

do_mach_notify_send_once

coalition_notification

coalition_notification_server

coalition_notification_server_routine

fairplay_server

fairplay_server_routine

fairplayd_arcade_request

receive_sysdiagnose_notification

receive_sysdiagnose_notification_with_audit_token

mach_dead_name_notification_t

mach_no_senders_notification_t

mach_send_once_notification_t

mach_send_possible_notification_t

### Ports

mem_entry_name_port_t

mach_port_array_t

mach_port_context_t

mach_port_delta_t

mach_port_flavor_t

mach_port_guard_exception_codes

mach_port_info_t

mach_port_mscount_t

mach_port_msgcount_t

mach_port_name_array_t

mach_port_name_t

mach_port_options_ptr_t

mach_port_right_t

mach_port_rights_t

mach_port_seqno_t

mach_port_srights_t

mach_port_t

mach_port_type_array_t

mach_port_type_t

mach_port_urefs_t

mach_port_allocate

mach_port_allocate_full

mach_port_allocate_name

mach_port_allocate_qos

mach_port_construct

mach_port_deallocate

mach_port_destroy

mach_port_destruct

mach_port_dnrequest_info

mach_port_extract_member

mach_port_extract_right

mach_port_get_attributes

mach_port_get_context

mach_port_get_refs

mach_port_get_set_status

mach_port_get_srights

mach_port_guard

mach_port_guard_with_flags

mach_port_insert_member

mach_port_insert_right

mach_port_kernel_object

mach_port_kobject

mach_port_kobject_description

mach_port_mod_refs

mach_port_move_member

mach_port_names

mach_port_peek

mach_port_rename

mach_port_request_notification

mach_port_set_attributes

mach_port_set_context

mach_port_set_mscount

mach_port_set_seqno

mach_port_space_basic_info

mach_port_space_info

mach_port_special_reply_port_reset_link

mach_port_swap_guard

mach_port_type

mach_port_unguard

mach_eventlink_t

audit_triggers

mach_port_deleted_notification_t

mach_port_destroyed_notification_t

mach_port_info_ext_t

mach_port_limits_t

mach_port_options_t

mach_port_qos_t

mach_port_status_t

ipc_info_name_array_t

ipc_info_tree_name_array_t

ipc_object_t

ipc_perm

ipc_port_t

ipc_pthread_priority_value_t

ipc_space_inspect_t

ipc_space_port_t

ipc_space_t

ipc_voucher_attr_control_t

ipc_voucher_attr_manager_t

ipc_voucher_t

### Processor

processor_assign

processor_control

processor_exit

processor_get_assignment

processor_info

processor_set_create

processor_set_default

processor_set_destroy

processor_set_info

processor_set_max_priority

processor_set_policy_control

processor_set_policy_disable

processor_set_policy_enable

processor_set_stack_usage

processor_set_statistics

processor_set_tasks

processor_set_threads

processor_start

### Semaphore

semaphore_create

semaphore_destroy

semaphore_signal

semaphore_signal_all

semaphore_wait

semaphore_wait_deadline

semaphore_wait_noblock

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

thread_set_thread_name

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

task_vm_info_data_t

task_wait_state_info_data_t

task_zone_info_t

check_task_access

### Time

mach_absolute_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), this clock does not increment while the system is asleep.

mach_approximate_time

mach_continuous_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), including while the system is asleep.

mach_continuous_approximate_time

mach_bridge_remote_time

mach_bridge_compute_timestamp

mach_bridge_register_regwrite_timestamp_callback

mach_timebase_info_t

mach_zone_info_array_t

mach_zone_name_array_t

mach_timebase_info_data_t

Raw Mach Time API In general prefer to use the \ API clock_gettime_nsec_np(3), which deals in the same clocks (and more) in ns units. Conversion of ns to (resp. from) tick units as returned by the mach time APIs is performed by division (resp. multiplication) with the fraction returned by mach_timebase_info().

mach_timespec_t

mach_zone_info_t

clock_attr_t

clock_ctrl_port_t

clock_ctrl_t

clock_flavor_t

clock_id_t

clock_nsec_t

clock_reply_subsystem

clock_reply_t

clock_res_t

clock_sec_t

clock_serv_port_t

clock_serv_t

clock_t

clock_usec_t

clockinfo

### Host

host_self

host_priv_self

host_reboot

host_processor_info

host_processor_set_priv

host_processor_sets

host_processors

host_request_notification

host_get_boot_info

host_lockgroup_info

host_info

host_kernel_version

host_statistics

host_statistics64

host_priv_statistics

host_set_UNDServer

host_get_UNDServer

host_get_clock_control

host_get_clock_service

host_set_atm_diagnostic_flag

host_set_multiuser_config_flags

host_security_create_task_token

host_security_set_task_token

host_virtual_physical_table_info

host_default_memory_manager

host_vmxoff

host_vmxon

host_page_size

host_get_exception_ports

host_get_special_port

host_set_exception_ports

host_set_special_port

host_swap_exception_ports

mach_zone_force_gc

mach_zone_get_btlog_records

mach_zone_get_zlog_zones

mach_zone_info

mach_zone_info_for_largest_zone

mach_zone_info_for_zone

processor_array_t

processor_basic_info_t

processor_cpu_load_info_t

processor_flavor_t

processor_info_array_t

processor_info_data_t

processor_info_t

processor_port_array_t

processor_port_t

processor_set_array_t

processor_set_basic_info_t

processor_set_control_port_t

processor_set_control_t

processor_set_flavor_t

processor_set_info_data_t

processor_set_info_t

processor_set_load_info_t

processor_set_name_array_t

processor_set_name_port_array_t

processor_set_name_port_t

processor_set_name_t

processor_set_port_t

processor_set_t

processor_t

host_basic_info_t

host_can_has_debugger_info_t

host_cpu_load_info_t

host_flavor_t

host_info64_t

host_info_data_t

host_info_t

host_load_info_t

host_name_port_t

host_name_t

host_preferred_user_arch_t

host_priority_info_t

host_priv_t

host_purgable_info_t

host_sched_info_t

host_security_t

host_t

policy_base_t

policy_fifo_base_t

policy_fifo_info_t

policy_fifo_limit_t

policy_info_t

policy_limit_t

policy_rr_base_t

policy_rr_info_t

policy_rr_limit_t

policy_t

policy_timeshare_base_t

policy_timeshare_info_t

policy_timeshare_limit_t

mach_zone_name_t

zone_btrecord_array_t

zone_info_array_t

zone_name_array_t

kmod_control

kmod_create

kmod_destroy

kmod_get_info

### Security

mach_gss_accept_sec_context

mach_gss_accept_sec_context_v2

mach_gss_hold_cred

mach_gss_init_sec_context

mach_gss_init_sec_context_v2

mach_gss_init_sec_context_v3

mach_gss_log_error

mach_gss_lookup

mach_gss_unhold_cred

### Voucher

mach_voucher_attr_command

mach_voucher_attr_control_create_mach_voucher

mach_voucher_attr_control_get_values

mach_voucher_debug_info

mach_voucher_extract_all_attr_recipes

mach_voucher_extract_attr_content

mach_voucher_extract_attr_recipe

host_create_mach_voucher

host_register_mach_voucher_attr_manager

host_register_well_known_mach_voucher_attr_manager

mach_voucher_attr_command_t

mach_voucher_attr_content_size_t

mach_voucher_attr_content_t

mach_voucher_attr_control_flags_t

mach_voucher_attr_control_t

mach_voucher_attr_importance_refs

mach_voucher_attr_key_array_t

mach_voucher_attr_key_t

mach_voucher_attr_manager_t

mach_voucher_attr_raw_recipe_array_size_t

mach_voucher_attr_raw_recipe_array_t

mach_voucher_attr_raw_recipe_size_t

mach_voucher_attr_raw_recipe_t

mach_voucher_attr_recipe_command_array_t

mach_voucher_attr_recipe_command_t

mach_voucher_attr_recipe_size_t

mach_voucher_attr_recipe_t

mach_voucher_attr_value_flags_t

mach_voucher_attr_value_handle_array_size_t

mach_voucher_attr_value_handle_array_t

mach_voucher_attr_value_handle_t

mach_voucher_attr_value_reference_t

mach_voucher_name_array_t

mach_voucher_name_t

mach_voucher_selector_t

mach_voucher_t

mach_voucher_attr_recipe_data_t

### i386

x86_avx512_state32_t

x86_avx512_state64_t

x86_avx512_state_t

x86_avx_state32_t

x86_avx_state64_t

x86_avx_state_t

x86_debug_state32_t

x86_debug_state64_t

x86_debug_state_t

x86_exception_state64_t

x86_exception_state_t

x86_float_state64_t

x86_float_state_t

x86_pagein_state_t

x86_state_hdr_t

x86_thread_full_state64_t

x86_thread_state64_t

x86_thread_state_t

### Errors

mach_to_bsd_errno

mach_error_fn_t

mach_error_t

mach_exception_code_t

mach_exception_data_t

mach_exception_data_type_t

mach_exception_subcode_t

exception_behavior_array_t

exception_behavior_t

exception_data_t

exception_data_type_t

exception_flavor_array_t

exception_handler_array_t

exception_handler_t

exception_mask_array_t

exception_mask_t

exception_port_arrary_t

exception_port_array_t

exception_port_t

exception_type_t

### Support

mach_atm_subaid_t

mach_core_details

mach_core_fileheader

mach_header

mach_header_64

mach_bridge_regwrite_timestamp_func_t

## See Also

### Mach

mach-o

Access interfaces associated with the Mach-O runtime.

