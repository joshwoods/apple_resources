

- Kernel
- Debugging
-  catch_mach_exception_raise_state 

Function

# catch_mach_exception_raise_state

macOS 10.5+

``` source
kern_return_t catch_mach_exception_raise_state(mach_port_t exception_port, exception_type_t exception, const mach_exception_data_t code, mach_msg_type_number_t codeCnt, int *flavor, const thread_state_t old_state, mach_msg_type_number_t old_stateCnt, thread_state_t new_state, mach_msg_type_number_t *new_stateCnt);
```

## See Also

### Exceptions

catch_exception_raise

catch_exception_raise_state

catch_exception_raise_state_identity

catch_mach_exception_raise

catch_mach_exception_raise_state_identity

