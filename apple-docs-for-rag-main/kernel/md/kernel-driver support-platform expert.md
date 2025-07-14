

- Kernel
- Driver Support
-  Platform Expert 

API Collection

# Platform Expert

## Topics

### Setup and Initialization

PE_init_cpu

PE_init_iokit

PE_init_panicheader

PE_init_platform

PE_init_printf

PE_init_taproot

PE_boot_args

PE_parse_boot_argn

PE_initialize_console

PE_install_interrupt_handler

PE_create_console

PE_current_console

### CPU

PE_cpu_halt

PE_cpu_machine_init

PE_cpu_machine_quiesce

PE_cpu_signal

PE_cpu_signal_cancel

PE_cpu_signal_deferred

PE_cpu_start

### Debugging

PE_i_can_has_debugger

PE_enter_debugger

PESavePanicInfo

PESavePanicInfoAction

PE_panic_hook

PE_update_panicheader_nestedpanic

PE_get_offset_into_panic_region

PEHaltRestart

### Configuration Details

PEGetCoprocessorVersion

PEGetGMTTimeOfDay

PEGetMachineName

PEGetModelName

PEGetPlatformEpoch

PEGetUTCTimeOfDay

PESetGMTTimeOfDay

PESetUTCTimeOfDay

PE_get_default

PE_get_hotkey

PE_get_random_seed

PE_register_timebase_callback

PE_call_timebase_callback

PE_display_icon

PE_imgsrc_mount_supported

PE_stub_poll_input

### NVRAM

PEReadNVRAMProperty

PERemoveNVRAMProperty

PEWriteNVRAMBooleanProperty

PEWriteNVRAMProperty

PEWriteNVRAMPropertyWithCopy

## See Also

### Default Devices

IOPlatformExpertDevice

IOPlatformDevice

Device Tree

