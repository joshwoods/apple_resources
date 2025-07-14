

- Kernel
- mach
-  processor_set_stack_usage 

Function

# processor_set_stack_usage

macOS 10.0+

``` source
kern_return_t processor_set_stack_usage(processor_set_t pset, unsigned int *ltotal, vm_size_t *space, vm_size_t *resident, vm_size_t *maxusage, vm_offset_t *maxstack);
```

## See Also

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

processor_set_statistics

processor_set_tasks

processor_set_threads

processor_start

