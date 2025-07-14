

- Kernel
- architecture
-  i386_cpu_info_t 

Structure

# i386_cpu_info_t

macOS 10.3+

``` source
typedef struct i386_cpu_info {
    ...
} i386_cpu_info_t;
```

## Topics

### Instance Properties

cache_info

cache_linesize

cache_partitions

cache_sharing

cache_size

core_count

cpuid_address_bits_physical

cpuid_address_bits_virtual

cpuid_arch_perf_leaf

cpuid_arch_perf_leafp

cpuid_brand

cpuid_brand_string

cpuid_cache_L2_associativity

cpuid_cache_linesize

cpuid_cache_size

cpuid_cores_per_package

cpuid_cpu_subtype

cpuid_cpu_type

cpuid_cpufamily

cpuid_extfamily

cpuid_extfeatures

cpuid_extmodel

cpuid_family

cpuid_features

cpuid_leaf7_extfeatures

cpuid_leaf7_features

cpuid_logical_per_package

cpuid_max_basic

cpuid_max_ext

cpuid_microcode_version

cpuid_model

cpuid_model_string

cpuid_mwait_leaf

cpuid_mwait_leafp

cpuid_processor_flag

cpuid_signature

cpuid_stepping

cpuid_stlb

cpuid_thermal_leaf

cpuid_thermal_leafp

cpuid_tlb

cpuid_tsc_leaf

cpuid_type

cpuid_vendor

cpuid_xsave_leaf

cpuid_xsave_leafp

thread_count

unused

## See Also

### i386

hlt

inb

do_cpuid

get_cr0

get_cr2

get_cr3_base

get_cr3_raw

get_cr4

get_crc_table

get_ds

get_es

get_fs

get_gs

get_ss

get_tr

cpuid

cpuid_cpu_display

cpuid_cpufamily

cpuid_cpusubtype

cpuid_cputype

cpuid_extfeature_display

cpuid_extfeatures

cpuid_family

cpuid_feature_display

cpuid_features

cpuid_get_extfeature_names

cpuid_get_feature_names

cpuid_get_leaf7_extfeature_names

cpuid_get_leaf7_feature_names

cpuid_info

cpuid_leaf7_extfeatures

cpuid_leaf7_features

cpuid_set_info

clac

clz

clear_ts

cninit

cpuid_arch_perf_leaf_t

cpuid_cache_desc_t

cpuid_mwait_leaf_t

cpuid_thermal_leaf_t

cpuid_tsc_leaf_t

cpuid_xsave_leaf_t

i386_exception_state_t

i386_float_state_t

i386_thread_state_t

