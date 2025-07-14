

- Hypervisor
-  hv_simd_fp_uchar16_t 

Type Alias

# hv_simd_fp_uchar16_t

The value that represents an ARM SIMD and FP register.

macOS

``` source
typealias hv_simd_fp_uchar16_t = SIMD16
```

## See Also

### SIMD &amp; Floating-point registers

func hv_vcpu_get_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, UnsafeMutablePointer&lt;hv_simd_fp_uchar16_t>) -> hv_return_t

Gets the current value of a vCPU SIMD and FP register.

func hv_vcpu_set_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, hv_simd_fp_uchar16_t) -> hv_return_t

Sets the value of a vCPU SIMD&FP register.

struct hv_simd_fp_reg_t

The type that defines SIMD and floating-point registers.

