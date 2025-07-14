

- Latent Semantic Mapping
-  LSMResultCreate(\_:\_:\_:\_:\_:) 

Function

# LSMResultCreate(\_:\_:\_:\_:\_:)

Returns the categories or words that best match when a text is mapped into a map, in decreasing order of likelihood.

Mac CatalystmacOS

``` source
func LSMResultCreate(
    _ alloc: CFAllocator?,
    _ mapref: LSMMap,
    _ textref: LSMText,
    _ numResults: CFIndex,
    _ flags: CFOptionFlags
) -> Unmanaged
```

## See Also

### Creating a Result

Result Flags

Options for creating a result.

