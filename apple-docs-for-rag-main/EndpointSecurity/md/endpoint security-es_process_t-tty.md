

- Endpoint Security
- es_process_t
-  tty 

Instance Property

# tty

The TTY associated with the process sending the message.

Mac CatalystmacOS

``` source
var tty: UnsafeMutablePointer?
```

## Discussion

This field is available if the message version is greater than `2`.

## See Also

### Inspecting Process IDs

var ppid: pid_t

The parent process identifier.

var original_ppid: pid_t

The original parent process ID.

var group_id: pid_t

The process group identifier.

var session_id: pid_t

The identifier of the session that contains the process group.

