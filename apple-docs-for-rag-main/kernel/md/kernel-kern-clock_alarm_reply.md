

- Kernel
- kern
-  clock_alarm_reply 

Function

# clock_alarm_reply

macOS 10.0+

``` source
kern_return_t clock_alarm_reply(clock_reply_t alarm_port, kern_return_t alarm_code, alarm_type_t alarm_type, mach_timespec_t alarm_time);
```

## See Also

### clock

continuoustime_to_absolutetime

clock_absolutetime_interval_to_deadline

clock_alarm

clock_continuoustime_interval_to_deadline

clock_delay_until

clock_get_attributes

clock_get_calendar_absolute_and_microtime

clock_get_calendar_microtime

clock_get_calendar_nanotime

clock_get_system_microtime

clock_get_system_nanotime

clock_get_time

clock_get_uptime

clock_interval_to_absolutetime_interval

clock_interval_to_deadline

clock_reply_server

clock_reply_server_routine

clock_set_attributes

clock_set_time

clock_timebase_info

absolutetime_to_continuoustime

absolutetime_to_nanoseconds

