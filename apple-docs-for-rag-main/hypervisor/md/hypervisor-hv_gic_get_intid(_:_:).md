

- Hypervisor
-  hv_gic_get_intid(\_:\_:) 

Function

# hv_gic_get_intid(\_:\_:)

Gets the interrupt ID for reserved interrupts.

macOS 15.0+

``` source
func hv_gic_get_intid(
    _ interrupt: hv_gic_intid_t,
    _ intid: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`interrupt`  

One of the hv_gic_intid_t values that represents a reserved interrupt.

`intid`  

A pointer to the interrupt number that the framework writes to upon success.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## See Also

### Reserved interrupt identifiers

var HV_GIC_INT_MAINTENANCE: hv_gic_intid_t

A register Hypervisor uses to signal virtual Interrupts (vIRQs) that the framework sends to guests running at exception level 2 (EL2).

var HV_GIC_INT_PERFORMANCE_MONITOR: hv_gic_intid_t

A register the framework uses to count GIC related events.

var HV_GIC_INT_EL1_PHYSICAL_TIMER: hv_gic_intid_t

var HV_GIC_INT_EL2_PHYSICAL_TIMER: hv_gic_intid_t

var HV_GIC_INT_EL1_VIRTUAL_TIMER: hv_gic_intid_t

