

- Kernel
- mach
-  processor_info 

Function

# processor_info

macOS 10.0+

``` source
kern_return_t processor_info(processor_t processor, processor_flavor_t flavor, host_t *host, processor_info_t processor_info_out, mach_msg_type_number_t *processor_info_outCnt);
```

## See Also

### Processor

processor_assign

processor_control

processor_exit

processor_get_assignment

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

