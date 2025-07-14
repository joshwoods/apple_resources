

- Latent Semantic Mapping
-  LSMMapSetProperties(\_:\_:) 

Function

# LSMMapSetProperties(\_:\_:)

Sets a dictionary of properties for the map.

Mac CatalystmacOS

``` source
func LSMMapSetProperties(
    _ mapref: LSMMap,
    _ properties: CFDictionary
)
```

## Discussion

Latent Semantic Mapping makes its own copy of the properties, so you don’t need to retain them past this call.

## See Also

### Managing a Map’s Properties

func LSMMapGetProperties(LSMMap) -> Unmanaged&lt;CFDictionary>

Gets a dictionary of properties for the map.

Map Properties

Special properties that determine a map’s behavior.

