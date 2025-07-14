

- Kernel
- Debugging
-  kernel_debug_enter 

Function

# kernel_debug_enter

macOS 10.15+

``` source
void kernel_debug_enter(uint32_t coreid, uint32_t debugid, uint64_t timestamp, uintptr_t arg1, uintptr_t arg2, uintptr_t arg3, uintptr_t arg4, uintptr_t threadid);
```

## See Also

### Kernel Debugging

Debugger

Enter the kernel debugger.

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

kernel_debug_filtered

kernel_debug_flags

kernel_debug_register_callbackDeprecated

