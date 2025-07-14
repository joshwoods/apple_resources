

- Latent Semantic Mapping
-  LSMMapCompile(\_:) 

Function

# LSMMapCompile(\_:)

Compiles the map into executable form and puts it into mapping mode, preparing it for the classification of texts.

Mac CatalystmacOS

``` source
func LSMMapCompile(_ mapref: LSMMap) -> OSStatus
```

## Discussion

This function is computationally expensive.

## See Also

### Starting Classification Mode

func LSMMapCreateClusters(CFAllocator?, LSMMap, CFArray?, CFIndex, CFOptionFlags) -> Unmanaged&lt;CFArray>?

Computes a set of clusters that group similar categories or words.

Clustering Flags

Options for creating clusters.

func LSMMapApplyClusters(LSMMap, CFArray) -> OSStatus

Groups categories or words (tokens) into the specified sets of clusters.

