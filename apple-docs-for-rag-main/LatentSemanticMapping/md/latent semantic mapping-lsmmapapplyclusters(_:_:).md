

- Latent Semantic Mapping
-  LSMMapApplyClusters(\_:\_:) 

Function

# LSMMapApplyClusters(\_:\_:)

Groups categories or words (tokens) into the specified sets of clusters.

Mac CatalystmacOS

``` source
func LSMMapApplyClusters(
    _ mapref: LSMMap,
    _ clusters: CFArray
) -> OSStatus
```

## See Also

### Starting Classification Mode

func LSMMapCompile(LSMMap) -> OSStatus

Compiles the map into executable form and puts it into mapping mode, preparing it for the classification of texts.

func LSMMapCreateClusters(CFAllocator?, LSMMap, CFArray?, CFIndex, CFOptionFlags) -> Unmanaged&lt;CFArray>?

Computes a set of clusters that group similar categories or words.

Clustering Flags

Options for creating clusters.

