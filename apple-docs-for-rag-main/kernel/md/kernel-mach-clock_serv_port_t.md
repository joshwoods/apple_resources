

- Kernel
- mach
-  clock_serv_port_t 

Type Alias

# clock_serv_port_t

macOS 10.0+

``` source
typedef clock_serv_t clock_serv_port_t;
```

## See Also

### Time

mach_absolute_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), this clock does not increment while the system is asleep.

mach_approximate_time

mach_continuous_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), including while the system is asleep.

mach_continuous_approximate_time

mach_bridge_remote_time

mach_bridge_compute_timestamp

mach_bridge_register_regwrite_timestamp_callback

mach_timebase_info_t

mach_zone_info_array_t

mach_zone_name_array_t

mach_timebase_info_data_t

Raw Mach Time API In general prefer to use the \ API clock_gettime_nsec_np(3), which deals in the same clocks (and more) in ns units. Conversion of ns to (resp. from) tick units as returned by the mach time APIs is performed by division (resp. multiplication) with the fraction returned by mach_timebase_info().

mach_timespec_t

mach_zone_info_t

clock_attr_t

clock_ctrl_port_t

clock_ctrl_t

clock_flavor_t

clock_id_t

clock_nsec_t

clock_reply_subsystem

clock_reply_t

clock_res_t

clock_sec_t

clock_serv_t

clock_t

clock_usec_t

clockinfo

