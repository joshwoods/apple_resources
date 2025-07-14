

- DriverKit
-  C++ Runtime Support 

API Collection

# C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

## Topics

### Object Support

OSObjectAllocate

Helper function for OSTypeAlloc(). Not to be called directly.

OSObjectRetain

OSObjectRelease

### Additional Types

IOReturn

IOOptionBits

integer_t

natural_t

kern_return_t

IOItemCount

IOVersion

### Log Support

OSObjectLog

IOLogBuffer

crc32

### Base Classes

OSMetaClass

Base class for DriverKit runtime class system. Not called directly.

OSMetaClassBase

Base class for DriverKit objects.

### RPC Support

IORPC

IORPCMessage

IORPCMessageMach

IORPCMessageErrorReturn

OSClassLoadInformation

OSClassDescription

OSDispatchMethod

RPC Message ID

RPC Message Types

RPC Capabilities

RPC Version

IORPCMessageFromMach

### Mach Ports

mach_port_name_t

mach_port_t

### Mach Timebase

mach_absolute_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), this clock does not increment while the system is asleep.

mach_continuous_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), including while the system is asleep.

mach_timebase_info

Returns fraction to multiply a value in mach tick units with to convert it to nanoseconds.

mach_timebase_info_t

Time Scales

### Mach Messages

mach_msg_bits_t

mach_msg_copy_options_t

mach_msg_descriptor_type_t

mach_msg_id_t

mach_msg_size_t

mach_msg_type_name_t

mach_msg_body_t

mach_msg_header_t

mach_msg_max_trailer_t

mach_msg_ool_descriptor_t

mach_msg_port_descriptor_t

mach_timebase_info_data_t

Raw Mach Time API In general prefer to use the \ API clock_gettime_nsec_np(3), which deals in the same clocks (and more) in ns units. Conversion of ns to (resp. from) tick units as returned by the mach time APIs is performed by division (resp. multiplication) with the fraction returned by mach_timebase_info().

### Boot Support

IOParseBootArgNumber

Parses any boot arguments in the macOS kernel boot-args.

IOParseBootArgString

Parses any boot arguments in the macOS kernel boot-args.

### Thread Utilities

IODelay

Sleep the calling thread for a number of microseconds.

IOSleep

Sleep the calling thread for a number of milliseconds.

### Additional Utilities

OSReportWithBacktrace

Generates a backtrace and message for debugging.

OSSynchronizeIO

Performs an `mfence` instruction on Intel-based Mac computers.

## See Also

### Runtime support

OSDynamicCast

Casts an object safely to the specified type, if possible.

OSRequiredCast

Casts the object to the specified type, stopping the process if the object isn’t of the correct type.

IMPL

Tells the system that the superclass implementation of this method runs in the kernel.

TYPE

Annotates a method declaration to indicate that it conforms to an existing method signature.

QUEUENAME

Tells the system to execute a method on the dispatch queue with the specified name.

SUPERDISPATCH

Tells the system to execute the superclass’ implementation of the current method in the kernel.

IIG_KERNEL

Tells the system that the class or method runs inside the kernel.

LOCAL

Tells the system that the method runs locally in the driver extension’s process space.

LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

Error Codes

Determine the reason an operation fails.

