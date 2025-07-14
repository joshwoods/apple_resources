

- Endpoint Security
- es_process_t
-  group_id 

Instance Property

# group_id

The process group identifier.

Mac CatalystmacOS

``` source
var group_id: pid_t
```

## See Also

### Inspecting Process IDs

var ppid: pid_t

The parent process identifier.

var original_ppid: pid_t

The original parent process ID.

var session_id: pid_t

The identifier of the session that contains the process group.

var tty: UnsafeMutablePointer&lt;es_file_t>?

The TTY associated with the process sending the message.

