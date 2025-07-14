

- Endpoint Security
-  es_invert_muting(\_:\_:) 

Function

# es_invert_muting(\_:\_:)

macOS 13.0+

``` source
func es_invert_muting(
    _ client: OpaquePointer,
    _ mute_type: es_mute_inversion_type_t
) -> es_return_t
```

## See Also

### Functions

func es_muting_inverted(OpaquePointer, es_mute_inversion_type_t) -> es_mute_inverted_return_t

func es_unmute_all_target_paths(OpaquePointer) -> es_return_t

