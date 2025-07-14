

- Kernel
- mach
-  mach_dead_name_notification_t 

Structure

# mach_dead_name_notification_t

macOS 10.0+

``` source
typedef struct mach_dead_name_notification_t {
    ...
} mach_dead_name_notification_t;
```

## Topics

### Instance Properties

NDR

not_header

not_port

trailer

## See Also

### Notifications

do_mach_notify_dead_name

do_mach_notify_no_senders

do_mach_notify_port_deleted

do_mach_notify_port_destroyed

do_mach_notify_send_once

coalition_notification

coalition_notification_server

coalition_notification_server_routine

fairplay_server

fairplay_server_routine

fairplayd_arcade_request

receive_sysdiagnose_notification

receive_sysdiagnose_notification_with_audit_token

mach_no_senders_notification_t

mach_send_once_notification_t

mach_send_possible_notification_t

