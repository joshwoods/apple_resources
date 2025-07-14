

- Hypervisor
-  OS_hv_vcpu_config 

Protocol

# OS_hv_vcpu_config

Configuration for a virtual CPU.

macOS

``` source
protocol OS_hv_vcpu_config : NSObjectProtocol
```

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuration

func hv_vcpu_config_create() -> hv_vcpu_config_t

Creates a vCPU configuration object.

func hv_vcpu_config_get_feature_reg(hv_vcpu_config_t, hv_feature_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of a feature register.

func hv_vcpu_config_get_ccsidr_el1_sys_reg_values(hv_vcpu_config_t, hv_cache_type_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the Cache Size ID Register (CCSIDR_EL1) values for the vCPU configuration and cache type you specify.

typealias hv_vcpu_config_t

The type that defines a vCPU configuration.

struct hv_feature_reg_t

The type that defines feature registers.

