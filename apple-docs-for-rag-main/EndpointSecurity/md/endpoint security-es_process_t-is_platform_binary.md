

- Endpoint Security
- es_process_t
-  is_platform_binary 

Instance Property

# is_platform_binary

A Boolean value that indicates whether the process is a platform binary.

Mac CatalystmacOS

``` source
var is_platform_binary: Bool
```

## Discussion

For the purposes of this value, a “platform binary” is one signed with Apple certificates.

## See Also

### Inspecting the Source Process

var audit_token: audit_token_t

A token for use with Basic Security Module auditing functions.

var executable: UnsafeMutablePointer&lt;es_file_t>

The file containing the executed process.

var is_es_client: Bool

A Boolean value that indicates whether the process connects to the Endpoint Security subsystem.

var start_time: timeval

The time the process started.

