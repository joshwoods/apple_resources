

- Latent Semantic Mapping
-  LSMMapGetProperties(\_:) 

Function

# LSMMapGetProperties(\_:)

Gets a dictionary of properties for the map.

Mac CatalystmacOS

``` source
func LSMMapGetProperties(_ mapref: LSMMap) -> Unmanaged
```

## Discussion

Latent Semantic Mapping retains ownership of this dictionary; don’t release it.

## See Also

### Managing a Map’s Properties

func LSMMapSetProperties(LSMMap, CFDictionary)

Sets a dictionary of properties for the map.

Map Properties

Special properties that determine a map’s behavior.

