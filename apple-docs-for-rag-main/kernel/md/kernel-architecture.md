

- Kernel
-  architecture 

API Collection

# architecture

Access machine-level and architectural information about the current platform.

## Topics

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

i386_cpu_info_t

i386_exception_state_t

i386_float_state_t

i386_thread_state_t

### EFI

EFI_CONFIGURATION_TABLE_32

EFI_CONFIGURATION_TABLE_64

EFI_GUID

EFI_MEMORY_DESCRIPTOR

EFI_RUNTIME_SERVICES_32

EFI_RUNTIME_SERVICES_64

EFI_SYSTEM_TABLE_32

EFI_SYSTEM_TABLE_64

EFI_TABLE_HEADER

EFI_TIME

EFI_TIME_CAPABILITIES

EfiMemoryRange

EFI_BOOLEAN

EFI_CHAR16

EFI_CHAR32

EFI_CHAR64

EFI_CHAR8

EFI_CONVERT_POINTER

EFI_GET_NEXT_HIGH_MONO_COUNT

EFI_GET_NEXT_VARIABLE_NAME

EFI_GET_TIME

EFI_GET_VARIABLE

EFI_GET_WAKEUP_TIME

EFI_HANDLE32

EFI_HANDLE64

EFI_INT16

EFI_INT32

EFI_INT64

EFI_INT8

EFI_PHYSICAL_ADDRESS

EFI_PTR32

EFI_PTR64

EFI_RESET_SYSTEM

EFI_SET_TIME

EFI_SET_VARIABLE

EFI_SET_VIRTUAL_ADDRESS_MAP

EFI_SET_WAKEUP_TIME

EFI_STATUS

EFI_UINT16

EFI_UINT32

EFI_UINT64

EFI_UINT8

EFI_UINTN

EFI_VIRTUAL_ADDRESS

## See Also

### BSD

bsm

Audit resource usage on the system.

hfs

Access HFS file-system data structures.

kern

Access kernel-level interfaces including clock, task, kernel extension, lock, and compression utilities.

Math

Perform mathematical operations and manipulate integer, float, and double values.

miscfs

Access device nodes and other file-system entities.

net

Access network-related utilities.

Strings

Compare, convert, and catenate strings and access the resulting content of those strings.

sys

Access general system utilities for time, file systems, and system information.

vfs

Access the virtual file-system interfaces.

vm

Interact with the virtual memory system.

