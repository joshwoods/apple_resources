

- Hypervisor
-  hv_vcpu_write_fpstate(\_:\_:\_:) 

Function

# hv_vcpu_write_fpstate(\_:\_:\_:)

Sets the architectural x86 floating point and SIMD state of a vCPU.

macOS 10.10+

``` source
func hv_vcpu_write_fpstate(
    _ vcpu: hv_vcpuid_t,
    _ buffer: UnsafeMutableRawPointer,
    _ size: Int
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`buffer`  

The new floating point and SIMD state.

`size`  

Size of the memory buffer in bytes.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

The XSAVE feature set of the host processor defines the structure and size of the returned buffer.

Important

This function must be called by the owning thread.

## See Also

### Floating Point (FP) State

func hv_vcpu_read_fpstate(hv_vcpuid_t, UnsafeMutableRawPointer, Int) -> hv_return_t

Returns, by reference, the current architectural x86 floating point and SIMD state of a vCPU.

