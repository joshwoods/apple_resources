

- Kernel
- mach
-  processor_set_threads 

Function

# processor_set_threads

macOS 10.0+

``` source
kern_return_t processor_set_threads(processor_set_t processor_set, thread_act_array_t *thread_list, mach_msg_type_number_t *thread_listCnt);
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

processor_set_stack_usage

processor_set_statistics

processor_set_tasks

processor_start

