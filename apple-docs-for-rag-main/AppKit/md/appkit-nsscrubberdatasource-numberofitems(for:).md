

- AppKit
- NSScrubberDataSource
-  numberOfItems(for:) 

Instance Method

# numberOfItems(for:)

Asks the data source for the number of items in the scrubber.

macOS 10.12.2+

``` source
@MainActor
func numberOfItems(for scrubber: NSScrubber) -> Int
```

**Required**

## Parameters 

`scrubber`  

The scrubber whose item count is being requested.

## Return Value

The number of items in the scrubber.

