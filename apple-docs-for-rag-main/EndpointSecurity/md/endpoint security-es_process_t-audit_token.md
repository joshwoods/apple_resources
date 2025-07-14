

- Endpoint Security
- es_process_t
-  audit_token 

Instance Property

# audit_token

A token for use with Basic Security Module auditing functions.

Mac CatalystmacOS

``` source
var audit_token: audit_token_t
```

## Discussion

Use this token with the functions defined in `libbsm.h` to extract values such as the process identifier (`PID`), user identifier (`UID`), and group identifier (`GID`).

## See Also

### Inspecting the Source Process

var executable: UnsafeMutablePointer&lt;es_file_t>

The file containing the executed process.

var is_es_client: Bool

A Boolean value that indicates whether the process connects to the Endpoint Security subsystem.

var is_platform_binary: Bool

A Boolean value that indicates whether the process is a platform binary.

var start_time: timeval

The time the process started.

