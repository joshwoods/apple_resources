

- Kernel
- Debugging
-  catch_exception_raise_state_identity 

Function

# catch_exception_raise_state_identity

macOS 10.0+

``` source
kern_return_t catch_exception_raise_state_identity(mach_port_t exception_port, mach_port_t thread, mach_port_t task, exception_type_t exception, exception_data_t code, mach_msg_type_number_t codeCnt, int *flavor, thread_state_t old_state, mach_msg_type_number_t old_stateCnt, thread_state_t new_state, mach_msg_type_number_t *new_stateCnt);
```

## See Also

### Exceptions

catch_exception_raise

catch_exception_raise_state

catch_mach_exception_raise

catch_mach_exception_raise_state

catch_mach_exception_raise_state_identity

