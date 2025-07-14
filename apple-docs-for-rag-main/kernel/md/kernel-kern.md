

- Kernel
-  kern 

API Collection

# kern

Access kernel-level interfaces including clock, task, kernel extension, lock, and compression utilities.

## Topics

### C Data

kcdata_bzero

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

### circle queue

circle_dequeue

circle_dequeue_head

circle_dequeue_tail

circle_enqueue_head

circle_enqueue_tail

circle_queue_empty

circle_queue_first

circle_queue_last

circle_queue_length

circle_queue_next

circle_queue_rotate_head_backward

circle_queue_rotate_head_forward

### clock

continuoustime_to_absolutetime

clock_absolutetime_interval_to_deadline

clock_alarm

clock_alarm_reply

clock_continuoustime_interval_to_deadline

clock_delay_until

clock_get_attributes

clock_get_calendar_absolute_and_microtime

clock_get_calendar_microtime

clock_get_calendar_nanotime

clock_get_system_microtime

clock_get_system_nanotime

clock_get_time

clock_get_uptime

clock_interval_to_absolutetime_interval

clock_interval_to_deadline

clock_reply_server

clock_reply_server_routine

clock_set_attributes

clock_set_time

clock_timebase_info

absolutetime_to_continuoustime

absolutetime_to_nanoseconds

### crc

crc32

### debug

kern_feature_override

### energy

io_rate_update

io_rate_update_register

gpu_accumulate_time

gpu_describe

gpu_fceiling_cb_register

gpu_submission_telemetry

### extmod

extmod_statistics_incr_task_for_pid

extmod_statistics_incr_thread_create

extmod_statistics_incr_thread_set_state

### hv

hv_ast_pending

hv_get_support

hv_get_task_target

hv_get_thread_target

hv_get_volatile_state

hv_release_callbacks

hv_release_traps

hv_set_callbacks

hv_set_task_target

hv_set_thread_target

hv_set_traps

hv_support_init

hv_suspend

hv_task_trap

hv_thread_trap

### kext

kext_alloc

kext_alloc_init

kext_free

kext_request

kextd_ping

OSKextCancelRequest

Cancels a pending user-space kext request without invoking the callback.

OSKextGetCurrentIdentifier

Returns the CFBundleIdentifier for the calling kext as a C string.

OSKextGetCurrentLoadTag

Returns the run-time load tag for the calling kext as an `OSKextLoadTag`.

OSKextGetCurrentVersionString

Returns the CFBundleVersion for the calling kext as a C string.

OSKextGrabPgoData

OSKextLoadKextWithIdentifier

Request that a kext be loaded.

OSKextReleaseKextWithLoadTag

Release a loaded kext based on its load tag.

OSKextRequestResource

Requests data from a nonlocalized resource file in a kext bundle on disk.

OSKextResetPgoCounters

OSKextResetPgoCountersLock

OSKextResetPgoCountersUnlock

OSKextRetainKextWithLoadTag

Retain a loaded kext based on its load tag, and enable autounload for that kext.

### kcs

kcs_get_elem_count

kcs_get_elem_size

kcs_set_elem_size

### kpc

kpc_arch_init

kpc_configurable_config_count

kpc_configurable_count

kpc_configurable_max

kpc_controls_counter

kpc_controls_fixed_counters

kpc_counterbuf_alloc

kpc_counterbuf_free

kpc_fixed_config_count

kpc_fixed_count

kpc_fixed_max

kpc_force_all_ctrs

kpc_force_all_ctrs_arch

kpc_get_actionid

kpc_get_all_cpus_counters

kpc_get_classes

kpc_get_config

kpc_get_config_count

kpc_get_configurable_config

kpc_get_configurable_counters

kpc_get_configurable_pmc_mask

kpc_get_counter_count

kpc_get_counterbuf_size

kpc_get_cpu_counters

kpc_get_curcpu_counters

kpc_get_curthread_counters

kpc_get_fixed_config

kpc_get_fixed_counters

kpc_get_force_all_ctrs

kpc_get_period

kpc_get_pmu_version

kpc_get_rawpmu_config

kpc_get_running

kpc_get_shadow_counters

kpc_get_thread_counting

kpc_idle

kpc_idle_exit

kpc_init

kpc_is_running_configurable

kpc_is_running_fixed

kpc_multiple_clients

kpc_pm_acknowledge

kpc_popcount

kpc_rawpmu_config_count

kpc_register_cpu

kpc_register_pm_handler

kpc_release_pm_counters

kpc_reserve_pm_counters

kpc_sample_kperf

kpc_set_actionid

kpc_set_config

kpc_set_config_arch

kpc_set_period

kpc_set_period_arch

kpc_set_running

kpc_set_running_arch

kpc_set_sw_inc

kpc_set_thread_counting

kpc_thread_ast_handler

kpc_thread_create

kpc_thread_destroy

kpc_unregister_cpu

### locks

lck_attr_alloc_init

lck_attr_cleardebug

lck_attr_free

lck_attr_setdebug

lck_attr_setdefault

lck_grp_alloc_init

lck_grp_attr_alloc_init

lck_grp_attr_free

lck_grp_attr_setdefault

lck_grp_attr_setstat

lck_grp_free

lck_mtx_alloc_init

lck_mtx_assert

lck_mtx_destroy

lck_mtx_free

lck_mtx_init

lck_mtx_lock

lck_mtx_sleep

lck_mtx_sleep_deadline

lck_mtx_unlock

lck_rw_alloc_init

lck_rw_destroy

lck_rw_free

lck_rw_init

lck_rw_lock

lck_rw_lock_exclusive

lck_rw_lock_exclusive_to_shared

lck_rw_lock_shared

lck_rw_lock_shared_to_exclusive

lck_rw_sleep

lck_rw_sleep_deadline

lck_rw_try_lock

lck_rw_unlock

lck_rw_unlock_exclusive

lck_rw_unlock_shared

lck_spin_alloc_init

lck_spin_destroy

lck_spin_free

lck_spin_init

lck_spin_lock

lck_spin_lock_grp

lck_spin_sleep

lck_spin_sleep_deadline

lck_spin_sleep_grp

lck_spin_unlock

### queue

dequeue_head

dequeue_tail

enqueue_head

enqueue_tail

### task

current_task

task_access_server

task_access_server_routine

task_assign

task_assign_default

task_create

task_deallocate

task_generate_corpse

task_get_assignment

task_get_dyld_image_infos

task_get_emulation_vector

task_get_exc_guard_behavior

task_get_exception_ports

task_get_mach_voucher

task_get_special_port

task_get_state

task_info

task_inspect

task_is_driver

task_ledgers_footprint

task_map_corpse_info

task_map_corpse_info_64

task_policy

task_policy_get

task_policy_set

task_purgable_info

task_reference

task_register_dyld_get_process_state

task_register_dyld_image_infos

task_register_dyld_set_dyld_state

task_register_dyld_shared_cache_image_info

task_restartable_ranges_register

task_restartable_ranges_synchronize

task_resume

task_resume2

task_sample

task_self_region_footprint

task_self_region_footprint_set

task_set_emulation

task_set_emulation_vector

task_set_exc_guard_behavior

task_set_exception_ports

task_set_info

task_set_mach_voucher

task_set_memory_ownership_transfer

task_set_phys_footprint_limit

task_set_policy

task_set_port_space

task_set_ras_pc

task_set_special_port

task_set_state

task_suspend

task_suspend2

task_suspension_token_deallocate

task_swap_exception_ports

task_swap_mach_voucher

task_terminate

task_threads

task_unregister_dyld_image_infos

task_wire

task_zone_info

### thread

kernel_thread_start

Create a kernel thread.

## See Also

### BSD

architecture

Access machine-level and architectural information about the current platform.

bsm

Audit resource usage on the system.

hfs

Access HFS file-system data structures.

Math

Perform mathematical operations and manipulate integer, float, and double values.

miscfs

Access device nodes and other file-system entities.

net

Access network-related utilities.

Strings

Compare, convert, and catenate strings and access the resulting content of those strings.

sys

Access general system utilities for time, file systems, and system information.

vfs

Access the virtual file-system interfaces.

vm

Interact with the virtual memory system.

