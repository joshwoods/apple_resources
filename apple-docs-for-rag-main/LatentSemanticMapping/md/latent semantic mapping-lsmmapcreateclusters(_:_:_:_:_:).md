

- Latent Semantic Mapping
-  LSMMapCreateClusters(\_:\_:\_:\_:\_:) 

Function

# LSMMapCreateClusters(\_:\_:\_:\_:\_:)

Computes a set of clusters that group similar categories or words.

Mac CatalystmacOS

``` source
func LSMMapCreateClusters(
    _ alloc: CFAllocator?,
    _ mapref: LSMMap,
    _ subset: CFArray?,
    _ numClusters: CFIndex,
    _ flags: CFOptionFlags
) -> Unmanaged?
```

## Discussion

If `subset` is non-`NULL`, this function only performs clustering on the categories or words in `subset`.

## See Also

### Starting Classification Mode

func LSMMapCompile(LSMMap) -> OSStatus

Compiles the map into executable form and puts it into mapping mode, preparing it for the classification of texts.

Clustering Flags

Options for creating clusters.

func LSMMapApplyClusters(LSMMap, CFArray) -> OSStatus

Groups categories or words (tokens) into the specified sets of clusters.

