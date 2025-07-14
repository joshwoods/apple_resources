

- Latent Semantic Mapping
-  kLSMMapDiscardCounts 

Global Variable

# kLSMMapDiscardCounts

An option that specifies not to keep counts.

Mac CatalystmacOS

``` source
var kLSMMapDiscardCounts: Int { get }
```

## Discussion

If you specify this option when loading the map, you must reload the map without this option before calling LSMMapStartTraining(_:).

If you specify this option when storing the map, the stored map can’t be retrained at all. This option can save a lot of memory or disk space.

## See Also

### Constants

var kLSMMapLoadMutable: Int

An option that specifies to load the map as mutable in training state.

var kLSMMapHashText: Int

An option that specifies to transform the text so it’s not human-readable.

