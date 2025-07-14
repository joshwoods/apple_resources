

- Endpoint Security
- es_process_t
-  start_time 

Instance Property

# start_time

The time the process started.

Mac CatalystmacOS

``` source
var start_time: timeval
```

## Discussion

This value represents the time that a fork call created the process.

This field is only available if the message version is `3` or greater.

## See Also

### Inspecting the Source Process

var audit_token: audit_token_t

A token for use with Basic Security Module auditing functions.

var executable: UnsafeMutablePointer&lt;es_file_t>

The file containing the executed process.

var is_es_client: Bool

A Boolean value that indicates whether the process connects to the Endpoint Security subsystem.

var is_platform_binary: Bool

A Boolean value that indicates whether the process is a platform binary.

