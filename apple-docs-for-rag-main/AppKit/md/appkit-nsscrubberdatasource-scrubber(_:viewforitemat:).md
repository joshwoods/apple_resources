

- AppKit
- NSScrubberDataSource
-  scrubber(\_:viewForItemAt:) 

Instance Method

# scrubber(\_:viewForItemAt:)

Asks the data source object for the view the corresponds to the specified item in the scrubber.

macOS 10.12.2+

``` source
@MainActor
func scrubber(
    _ scrubber: NSScrubber,
    viewForItemAt index: Int
) -> NSScrubberItemView
```

**Required**

## Parameters 

`scrubber`  

The scrubber requesting the view.

`index`  

The index that specifies the location of the item in the scrubber.

## Return Value

A configured item view object.

