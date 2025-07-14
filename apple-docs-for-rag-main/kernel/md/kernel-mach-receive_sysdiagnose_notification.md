

- Kernel
- mach
-  receive_sysdiagnose_notification 

Function

# receive_sysdiagnose_notification

macOS 10.11+

``` source
kern_return_t receive_sysdiagnose_notification(mach_port_t sysdiagnose_port, uint32_t flags);
```

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

receive_sysdiagnose_notification_with_audit_token

mach_dead_name_notification_t

mach_no_senders_notification_t

mach_send_once_notification_t

mach_send_possible_notification_t

