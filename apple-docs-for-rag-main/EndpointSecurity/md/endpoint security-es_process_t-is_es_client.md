

- Endpoint Security
- es_process_t
-  is_es_client 

Instance Property

# is_es_client

A Boolean value that indicates whether the process connects to the Endpoint Security subsystem.

Mac CatalystmacOS

``` source
var is_es_client: Bool
```

## See Also

### Inspecting the Source Process

var audit_token: audit_token_t

A token for use with Basic Security Module auditing functions.

var executable: UnsafeMutablePointer&lt;es_file_t>

The file containing the executed process.

var is_platform_binary: Bool

A Boolean value that indicates whether the process is a platform binary.

var start_time: timeval

The time the process started.

