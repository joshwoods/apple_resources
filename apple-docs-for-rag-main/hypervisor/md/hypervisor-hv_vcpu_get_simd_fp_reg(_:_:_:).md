

- Hypervisor
-  hv_vcpu_get_simd_fp_reg(\_:\_:\_:) 

Function

# hv_vcpu_get_simd_fp_reg(\_:\_:\_:)

Gets the current value of a vCPU SIMD and FP register.

macOS 11.0+

``` source
func hv_vcpu_get_simd_fp_reg(
    _ vcpu: hv_vcpu_t,
    _ reg: hv_simd_fp_reg_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`vcpu`  

The vCPU instance.

`reg`  

The ID of the SIMD and FP register.

`value`  

The value of the register `reg` on output.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### SIMD &amp; Floating-point registers

func hv_vcpu_set_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, hv_simd_fp_uchar16_t) -> hv_return_t

Sets the value of a vCPU SIMD&FP register.

typealias hv_simd_fp_uchar16_t

The value that represents an ARM SIMD and FP register.

struct hv_simd_fp_reg_t

The type that defines SIMD and floating-point registers.

