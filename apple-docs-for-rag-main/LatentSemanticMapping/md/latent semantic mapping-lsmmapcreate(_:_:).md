

- Latent Semantic Mapping
-  LSMMapCreate(\_:\_:) 

Function

# LSMMapCreate(\_:\_:)

Creates a new Latent Semantic Mapping map.

Mac CatalystmacOS

``` source
func LSMMapCreate(
    _ alloc: CFAllocator?,
    _ flags: CFOptionFlags
) -> Unmanaged
```

## Discussion

Call CFRelease to dispose of the map.

## See Also

### Creating a Map

Map Flags

Options for creating a map.

