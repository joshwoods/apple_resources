

- Kernel
- kern
-  task_get_exc_guard_behavior 

Function

# task_get_exc_guard_behavior

macOS 10.15+

``` source
kern_return_t task_get_exc_guard_behavior(task_inspect_t task, task_exc_guard_behavior_t *behavior);
```

## See Also

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

