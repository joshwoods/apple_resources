

- Endpoint Security
- es_process_t
-  original_ppid 

Instance Property

# original_ppid

The original parent process ID.

Mac CatalystmacOS

``` source
var original_ppid: pid_t
```

## Discussion

This field stays constant, even if the process’ parent changes.

## See Also

### Inspecting Process IDs

var ppid: pid_t

The parent process identifier.

var group_id: pid_t

The process group identifier.

var session_id: pid_t

The identifier of the session that contains the process group.

var tty: UnsafeMutablePointer&lt;es_file_t>?

The TTY associated with the process sending the message.

