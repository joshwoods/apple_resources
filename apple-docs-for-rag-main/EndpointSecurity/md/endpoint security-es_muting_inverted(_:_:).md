

- Endpoint Security
-  es_muting_inverted(\_:\_:) 

Function

# es_muting_inverted(\_:\_:)

macOS 13.0+

``` source
func es_muting_inverted(
    _ client: OpaquePointer,
    _ mute_type: es_mute_inversion_type_t
) -> es_mute_inverted_return_t
```

## See Also

### Functions

func es_invert_muting(OpaquePointer, es_mute_inversion_type_t) -> es_return_t

func es_unmute_all_target_paths(OpaquePointer) -> es_return_t

