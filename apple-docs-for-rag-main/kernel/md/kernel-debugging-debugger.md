

- Kernel
- Debugging
-  Debugger 

Function

# Debugger

Enter the kernel debugger.

macOS 10.0+

``` source
void Debugger(const char *reason);
```

## Parameters 

`reason`  

A C-string to describe why the debugger is being entered.

## Discussion

This function freezes the kernel and enters the builtin debugger. It may not be possible to exit the debugger without a second machine.

## See Also

### Kernel Debugging

kdbg_get_cpu

kdbg_get_timestamp

kdbg_set_cpu

kdbg_set_timestamp

kdbg_set_timestamp_and_cpu

kdebug_commpage_state

kdebug_debugid_enabled

kdebug_debugid_explicitly_enabled

kdebug_using_continuous_time

kernel_debug

kernel_debug1

kernel_debug_enter

kernel_debug_filtered

kernel_debug_flags

kernel_debug_register_callbackDeprecated

