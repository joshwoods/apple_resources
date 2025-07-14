

- Kernel
-  Debugging 

API Collection

# Debugging

Debug your kernel extensions using the kernel debugger, assertions, exceptions, backtraces, and logging.

## Topics

### Kernel Debugging

Debugger

Enter the kernel debugger.

kdbg_get_cpu

kdbg_get_timestamp

kdbg_set_cpu

kdbg_set_timestamp

kdbg_set_timestamp_and_cpu

kdebug_commpage_state

kdebug_debugid_enabled

kdebug_debugid_explicitly_enabled

kdebug_using_continuous_time

kernel_debug

kernel_debug1

kernel_debug_enter

kernel_debug_filtered

kernel_debug_flags

kernel_debug_register_callbackDeprecated

### kdp

kdp_register_callout

kdp_register_send_receive

kdp_unregister_send_receive

### Assertions

Assert

assert_wait

assert_wait_deadline

assert_wait_deadline_with_leeway

assert_wait_timeout

assert_wait_timeout_with_leeway

### Backtrace

backtrace

backtrace_user

OSReportWithBacktrace

OSBacktrace

OSPrintBacktrace

### Exceptions

catch_exception_raise

catch_exception_raise_state

catch_exception_raise_state_identity

catch_mach_exception_raise

catch_mach_exception_raise_state

catch_mach_exception_raise_state_identity

### Logging

OS_os_log

IOLog

Log a message to console in text mode, and /var/log/system.log.

IOLogv

Log a message to console in text mode, and /var/log/system.log.

os_log_create

Creates a custom log object, to be passed to logging functions for sending messages to the logging system.

os_log_debug_enabled

Returns a Boolean value indicating whether debug-level logging is enabled for a specified log object.

os_log_info_enabled

Returns a Boolean value indicating whether info-level logging is enabled for a specified log object.

### Helpers

OSPrintMemory

IOFindNameForValue

IOFindValueForName

## See Also

### Utilities

AppleDSP

Perform digital signal processing on data.

