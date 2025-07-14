

- Kernel
- mach
-  mach_absolute_time 

Function

# mach_absolute_time

Returns current value of a clock that increments monotonically in tick units (starting at an arbitrary point), this clock does not increment while the system is asleep.

macOS 10.0+

``` source
uint64_t mach_absolute_time(void);
```

## Return Value

Value of mach absolute time clock.

## Discussion

Prefer to use the equivalent clock_gettime_nsec_np(CLOCK_UPTIME_RAW) in nanoseconds.

Important

This API has the potential of being misused to access device signals to try to identify the device or user, also known as fingerprinting. Regardless of whether a user gives your app permission to track, fingerprinting is not allowed. When you use this API in your app or third-party SDK (an SDK not provided by Apple), declare your usage and the reason for using the API in your app or third-party SDK’s `PrivacyInfo.xcprivacy` file. For more information, including the list of valid reasons for using the API, see Describing use of required reason API.

## See Also

### Time

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

clock_serv_port_t

clock_serv_t

clock_t

clock_usec_t

clockinfo

