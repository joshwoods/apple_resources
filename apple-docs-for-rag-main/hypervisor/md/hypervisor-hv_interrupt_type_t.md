

- Hypervisor
-  hv_interrupt_type_t 

Structure

# hv_interrupt_type_t

The type that defines the vCPU’s interrupts.

macOS

``` source
struct hv_interrupt_type_t
```

## Overview

To raise interrupts on a vCPU, call hv_vcpu_set_pending_interrupt(_:_:_:) prior to calling hv_vcpu_run(_:).

## Topics

### Instance properties

var rawValue: UInt32

An unisgned 32-bit integer that describes the interrupts.

### Initializers

init(UInt32)

Creates a new interrupt instance with the value you provide.

init(rawValue: UInt32)

Creates a new interrupt instance with the integer value you provide.

### Interrupt levels

var HV_INTERRUPT_TYPE_FIQ: hv_interrupt_type_t

ARM Fast Interrupt Request.

var HV_INTERRUPT_TYPE_IRQ: hv_interrupt_type_t

ARM Interrupt Request.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Runtime

func hv_vcpu_run(hv_vcpuid_t) -> hv_return_t

Starts the execution of a vCPU.

func hv_vcpus_exit(UnsafeMutablePointer&lt;hv_vcpu_t>, UInt32) -> hv_return_t

Forces an immediate exit of a set of vCPUs of the VM.

func hv_vcpu_get_pending_interrupt(hv_vcpu_t, hv_interrupt_type_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets pending interrupts for a vCPU.

func hv_vcpu_set_pending_interrupt(hv_vcpu_t, hv_interrupt_type_t, Bool) -> hv_return_t

Sets pending interrupts for a vCPU.

func hv_vcpu_get_exec_time(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the cumulative execution time of a vCPU, in nanoseconds.

Exits

Describe virtual machine exit conditions.

