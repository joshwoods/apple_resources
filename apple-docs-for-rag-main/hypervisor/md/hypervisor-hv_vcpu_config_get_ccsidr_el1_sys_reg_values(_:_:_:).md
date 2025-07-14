

- Hypervisor
-  hv_vcpu_config_get_ccsidr_el1_sys_reg_values(\_:\_:\_:) 

Function

# hv_vcpu_config_get_ccsidr_el1_sys_reg_values(\_:\_:\_:)

Returns the Cache Size ID Register (CCSIDR_EL1) values for the vCPU configuration and cache type you specify.

macOS 11.0+

``` source
func hv_vcpu_config_get_ccsidr_el1_sys_reg_values(
    _ config: hv_vcpu_config_t,
    _ cache_type: hv_cache_type_t,
    _ values: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`config`  

The vCPU configuration.

`cache_type`  

The cache type from the available hv_cache_type_t types.

`values`  

A pointer to the location for the return values.

## Return Value

A hv_return_t value that indicates that result of the function.

## See Also

### Configuration

func hv_vcpu_config_create() -> hv_vcpu_config_t

Creates a vCPU configuration object.

func hv_vcpu_config_get_feature_reg(hv_vcpu_config_t, hv_feature_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of a feature register.

typealias hv_vcpu_config_t

The type that defines a vCPU configuration.

protocol OS_hv_vcpu_config

Configuration for a virtual CPU.

struct hv_feature_reg_t

The type that defines feature registers.

