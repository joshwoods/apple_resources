

- ContactProvider
- ContactItemSyncAnchor
-  init(generationMarker:offset:) 

Initializer

# init(generationMarker:offset:)

Creates a sync anchor with the given generation marker and offset.

iOS 18.0+iPadOS 18.0+

``` source
init(
    generationMarker: Data,
    offset: Int
)
```

## Parameters 

`generationMarker`  

A marker that indicates the database generation being enumerated for changes.

`offset`  

An offset from the generation marker.

