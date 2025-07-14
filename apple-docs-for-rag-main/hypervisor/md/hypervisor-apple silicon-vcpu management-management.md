

- Hypervisor
- Apple Silicon
-  vCPU Management 

API Collection

# vCPU Management

Create and run virtual CPUs, and manage CPU-specific registers and features.

## Overview

Hypervisor creates Virtual CPUs with hv_vcpu_create(_:_:). Call functions that operate on the vCPU from the same thread with the exception of hv_vcpus_exit(_:_:).

Enter the vCPU by using hv_vcpu_run(_:). The function runs until the guest traps or an other thread calls hv_vcpus_exit(_:_:). On exit, hv_vcpu_run(_:) populates the hv_vcpu_exit_t with the exit reason.

Warning

Don’t use vCPUs on dispatch queues, because work from a single queue can run on different threads.

## Topics

### Configuration

func hv_vcpu_config_create() -> hv_vcpu_config_t

Creates a vCPU configuration object.

func hv_vcpu_config_get_feature_reg(hv_vcpu_config_t, hv_feature_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of a feature register.

func hv_vcpu_config_get_ccsidr_el1_sys_reg_values(hv_vcpu_config_t, hv_cache_type_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the Cache Size ID Register (CCSIDR_EL1) values for the vCPU configuration and cache type you specify.

typealias hv_vcpu_config_t

The type that defines a vCPU configuration.

protocol OS_hv_vcpu_config

Configuration for a virtual CPU.

struct hv_feature_reg_t

The type that defines feature registers.

### Creation and destruction

func hv_vm_get_max_vcpu_count(UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Returns the maximum number of vCPUs that the hypervisor supports.

func hv_vcpu_create(UnsafeMutablePointer&lt;hv_vcpuid_t>, hv_vcpu_options_t) -> hv_return_t

Creates a vCPU instance for the current thread.

func hv_vcpu_destroy(hv_vcpuid_t) -> hv_return_t

Destroys the vCPU instance associated with the current thread.

typealias hv_vcpu_t

An opaque value that represents a vCPU instance.

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

struct hv_interrupt_type_t

The type that defines the vCPU’s interrupts.

Exits

Describe virtual machine exit conditions.

### General registers

func hv_vcpu_get_reg(hv_vcpu_t, hv_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the current value of a vCPU register.

func hv_vcpu_set_reg(hv_vcpu_t, hv_reg_t, UInt64) -> hv_return_t

Sets the value of a vCPU register.

struct hv_reg_t

The type that defines general registers.

### SIMD &amp; Floating-point registers

func hv_vcpu_get_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, UnsafeMutablePointer&lt;hv_simd_fp_uchar16_t>) -> hv_return_t

Gets the current value of a vCPU SIMD and FP register.

func hv_vcpu_set_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, hv_simd_fp_uchar16_t) -> hv_return_t

Sets the value of a vCPU SIMD&FP register.

typealias hv_simd_fp_uchar16_t

The value that represents an ARM SIMD and FP register.

struct hv_simd_fp_reg_t

The type that defines SIMD and floating-point registers.

### System registers

func hv_vcpu_get_sys_reg(hv_vcpu_t, hv_sys_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the current value of a vCPU system register.

func hv_vcpu_set_sys_reg(hv_vcpu_t, hv_sys_reg_t, UInt64) -> hv_return_t

Sets the value of a vCPU system register.

struct hv_sys_reg_t

The type of system registers.

### Trap configuration

func hv_vcpu_get_trap_debug_exceptions(hv_vcpu_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets whether debug exceptions exit the guest.

func hv_vcpu_set_trap_debug_exceptions(hv_vcpu_t, Bool) -> hv_return_t

Sets whether debug exceptions exit the guest.

func hv_vcpu_get_trap_debug_reg_accesses(hv_vcpu_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets whether debug-register accesses exit the guest.

func hv_vcpu_set_trap_debug_reg_accesses(hv_vcpu_t, Bool) -> hv_return_t

Sets whether debug-register accesses exit the guest.

## See Also

### Resource management

Memory management

Map memory into the physical address space of the virtual machine.

