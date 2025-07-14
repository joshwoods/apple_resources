

- ContactProvider
- ContactItemSyncAnchor
-  offset 

Instance Property

# offset

An offset from the anchor’s generation marker.

iOS 18.0+iPadOS 18.0+

``` source
var offset: Int
```

## Discussion

You can use the offset to track a contiguous number of contact items you’ve successfully enumerated within the database generation.

## See Also

### Inspecting sync anchor properties

var generationMarker: Data

A value specific to your data source identifying the database generation you’re enumerating for changes.

