

- Hypervisor
-  hv_simd_fp_reg_t 

Structure

# hv_simd_fp_reg_t

The type that defines SIMD and floating-point registers.

macOS

``` source
struct hv_simd_fp_reg_t
```

## Topics

### SIMD and Floating-point registers

var HV_SIMD_FP_REG_Q0: hv_simd_fp_reg_t

The value representing SIMD register Q0.

var HV_SIMD_FP_REG_Q1: hv_simd_fp_reg_t

The value representing SIMD register Q1.

var HV_SIMD_FP_REG_Q2: hv_simd_fp_reg_t

The value representing SIMD register Q2.

var HV_SIMD_FP_REG_Q3: hv_simd_fp_reg_t

The value representing SIMD register Q3.

var HV_SIMD_FP_REG_Q4: hv_simd_fp_reg_t

The value representing SIMD register Q4.

var HV_SIMD_FP_REG_Q5: hv_simd_fp_reg_t

The value representing SIMD register Q5.

var HV_SIMD_FP_REG_Q6: hv_simd_fp_reg_t

The value representing SIMD register Q6.

var HV_SIMD_FP_REG_Q7: hv_simd_fp_reg_t

The value representing SIMD register Q7.

var HV_SIMD_FP_REG_Q8: hv_simd_fp_reg_t

The value representing SIMD register Q8.

var HV_SIMD_FP_REG_Q9: hv_simd_fp_reg_t

The value representing SIMD register Q9.

var HV_SIMD_FP_REG_Q10: hv_simd_fp_reg_t

The value representing SIMD register Q10.

var HV_SIMD_FP_REG_Q11: hv_simd_fp_reg_t

The value representing SIMD register Q11.

var HV_SIMD_FP_REG_Q12: hv_simd_fp_reg_t

The value representing SIMD register Q12.

var HV_SIMD_FP_REG_Q13: hv_simd_fp_reg_t

The value representing SIMD register Q13.

var HV_SIMD_FP_REG_Q14: hv_simd_fp_reg_t

The value representing SIMD register Q14.

var HV_SIMD_FP_REG_Q15: hv_simd_fp_reg_t

The value representing SIMD register Q15.

var HV_SIMD_FP_REG_Q16: hv_simd_fp_reg_t

The value representing SIMD register Q16.

var HV_SIMD_FP_REG_Q17: hv_simd_fp_reg_t

The value representing SIMD register Q17.

var HV_SIMD_FP_REG_Q18: hv_simd_fp_reg_t

The value representing SIMD register Q18.

var HV_SIMD_FP_REG_Q19: hv_simd_fp_reg_t

The value representing SIMD register Q19.

var HV_SIMD_FP_REG_Q20: hv_simd_fp_reg_t

The value representing SIMD register Q20.

var HV_SIMD_FP_REG_Q21: hv_simd_fp_reg_t

The value representing SIMD register Q21.

var HV_SIMD_FP_REG_Q22: hv_simd_fp_reg_t

The value representing SIMD register Q22.

var HV_SIMD_FP_REG_Q23: hv_simd_fp_reg_t

The value representing SIMD register Q23.

var HV_SIMD_FP_REG_Q24: hv_simd_fp_reg_t

The value representing SIMD register Q24.

var HV_SIMD_FP_REG_Q25: hv_simd_fp_reg_t

The value representing SIMD register Q25.

var HV_SIMD_FP_REG_Q26: hv_simd_fp_reg_t

The value representing SIMD register Q26.

var HV_SIMD_FP_REG_Q27: hv_simd_fp_reg_t

The value representing SIMD register Q27.

var HV_SIMD_FP_REG_Q28: hv_simd_fp_reg_t

The value representing SIMD register Q28.

var HV_SIMD_FP_REG_Q29: hv_simd_fp_reg_t

The value representing SIMD register Q29.

var HV_SIMD_FP_REG_Q30: hv_simd_fp_reg_t

The value representing SIMD register Q30.

var HV_SIMD_FP_REG_Q31: hv_simd_fp_reg_t

The value representing SIMD register Q31.

### Instance properties

var rawValue: UInt32

An unsigned 32-bit integer that represents SIMD and floating-point registers.

### Initializers

init(UInt32)

Creates a new SIMD and floating-point register instance.

init(rawValue: UInt32)

Creates a new SIMD and floating-point register instance.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### SIMD &amp; Floating-point registers

func hv_vcpu_get_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, UnsafeMutablePointer&lt;hv_simd_fp_uchar16_t>) -> hv_return_t

Gets the current value of a vCPU SIMD and FP register.

func hv_vcpu_set_simd_fp_reg(hv_vcpu_t, hv_simd_fp_reg_t, hv_simd_fp_uchar16_t) -> hv_return_t

Sets the value of a vCPU SIMD&FP register.

typealias hv_simd_fp_uchar16_t

The value that represents an ARM SIMD and FP register.

