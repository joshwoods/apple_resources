

- Kernel
- Debugging
-  catch_exception_raise 

Function

# catch_exception_raise

macOS 10.0+

``` source
kern_return_t catch_exception_raise(mach_port_t exception_port, mach_port_t thread, mach_port_t task, exception_type_t exception, exception_data_t code, mach_msg_type_number_t codeCnt);
```

## See Also

### Exceptions

catch_exception_raise_state

catch_exception_raise_state_identity

catch_mach_exception_raise

catch_mach_exception_raise_state

catch_mach_exception_raise_state_identity

