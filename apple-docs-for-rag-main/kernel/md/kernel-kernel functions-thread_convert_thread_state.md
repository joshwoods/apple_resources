

- Kernel
- Kernel Functions
-  thread_convert_thread_state 

Function

# thread_convert_thread_state

macOS 11.0+

``` source
kern_return_t thread_convert_thread_state(thread_act_t thread, int direction, thread_state_flavor_t flavor, thread_state_t in_state, mach_msg_type_number_t in_stateCnt, thread_state_t out_state, mach_msg_type_number_t *out_stateCnt);
```

