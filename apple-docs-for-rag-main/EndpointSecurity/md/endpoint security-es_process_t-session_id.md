

- Endpoint Security
- es_process_t
-  session_id 

Instance Property

# session_id

The identifier of the session that contains the process group.

Mac CatalystmacOS

``` source
var session_id: pid_t
```

## See Also

### Inspecting Process IDs

var ppid: pid_t

The parent process identifier.

var original_ppid: pid_t

The original parent process ID.

var group_id: pid_t

The process group identifier.

var tty: UnsafeMutablePointer&lt;es_file_t>?

The TTY associated with the process sending the message.

