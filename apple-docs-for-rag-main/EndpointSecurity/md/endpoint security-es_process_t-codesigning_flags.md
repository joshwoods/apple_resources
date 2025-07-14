

- Endpoint Security
- es_process_t
-  codesigning_flags 

Instance Property

# codesigning_flags

The flags used to sign the process.

Mac CatalystmacOS

``` source
var codesigning_flags: UInt32
```

## Discussion

See `kern/cs_blobs.h` in the macOS SDK inside of the Xcode app bundle for definitions of these flags.

## See Also

### Inspecting Code Signing Properties

var cdhash: es_cdhash_t

The code directory hash value.

var signing_id: es_string_token_t

The identifier used to sign the process.

var team_id: es_string_token_t

The team identifier used to sign the process.

