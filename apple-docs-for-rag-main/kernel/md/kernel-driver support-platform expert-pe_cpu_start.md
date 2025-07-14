

- Kernel
- Driver Support
- Platform Expert
-  PE_cpu_start 

Function

# PE_cpu_start

macOS 10.0+

``` source
kern_return_t PE_cpu_start(cpu_id_t target, vm_offset_t start_paddr, vm_offset_t arg_paddr);
```

## See Also

### CPU

PE_cpu_halt

PE_cpu_machine_init

PE_cpu_machine_quiesce

PE_cpu_signal

PE_cpu_signal_cancel

PE_cpu_signal_deferred

