

- DriverKit
-  mach_msg_ool_descriptor_t 

Structure

# mach_msg_ool_descriptor_t

DriverKitiOSiPadOSmacOS

``` source
typedef struct { ... } mach_msg_ool_descriptor_t;
```

## Topics

### Getting the Properties

address

copy

deallocate

pad1

size

type

## See Also

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

mach_msg_port_descriptor_t

mach_timebase_info_data_t

Raw Mach Time API In general prefer to use the \ API clock_gettime_nsec_np(3), which deals in the same clocks (and more) in ns units. Conversion of ns to (resp. from) tick units as returned by the mach time APIs is performed by division (resp. multiplication) with the fraction returned by mach_timebase_info().

