

- Endpoint Security
- es_process_t
-  ppid 

Instance Property

# ppid

The parent process identifier.

Mac CatalystmacOS

``` source
var ppid: pid_t
```

## See Also

### Inspecting Process IDs

var original_ppid: pid_t

The original parent process ID.

var group_id: pid_t

The process group identifier.

var session_id: pid_t

The identifier of the session that contains the process group.

var tty: UnsafeMutablePointer&lt;es_file_t>?

The TTY associated with the process sending the message.

