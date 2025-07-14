

- Hypervisor
-  hv_vcpu_config_get_feature_reg(\_:\_:\_:) 

Function

# hv_vcpu_config_get_feature_reg(\_:\_:\_:)

Gets the value of a feature register.

macOS 11.0+

``` source
func hv_vcpu_config_get_feature_reg(
    _ config: hv_vcpu_config_t,
    _ feature_reg: hv_feature_reg_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`config`  

The vCPU configuration.

`feature_reg`  

The ID of the feature register.

`value`  

The value of `feature_reg` on output. Undefined if the call doesn’t succeed.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Configuration

func hv_vcpu_config_create() -> hv_vcpu_config_t

Creates a vCPU configuration object.

func hv_vcpu_config_get_ccsidr_el1_sys_reg_values(hv_vcpu_config_t, hv_cache_type_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the Cache Size ID Register (CCSIDR_EL1) values for the vCPU configuration and cache type you specify.

typealias hv_vcpu_config_t

The type that defines a vCPU configuration.

protocol OS_hv_vcpu_config

Configuration for a virtual CPU.

struct hv_feature_reg_t

The type that defines feature registers.

