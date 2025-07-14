

- Endpoint Security
- es_process_t
-  cdhash 

Instance Property

# cdhash

The code directory hash value.

Mac CatalystmacOS

``` source
var cdhash: es_cdhash_t
```

## Discussion

The code directory hash identifies a specific version of a program. This allows the system to verify that the contents of a binary have not changed since being code-signed.

## See Also

### Inspecting Code Signing Properties

var codesigning_flags: UInt32

The flags used to sign the process.

var signing_id: es_string_token_t

The identifier used to sign the process.

var team_id: es_string_token_t

The team identifier used to sign the process.

