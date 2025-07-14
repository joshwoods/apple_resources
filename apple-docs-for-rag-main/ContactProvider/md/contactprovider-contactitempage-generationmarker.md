

- ContactProvider
- ContactItemPage
-  generationMarker 

Instance Property

# generationMarker

A value specific to your data source identifying the database generation when enumeration of content started.

iOS 18.0+iPadOS 18.0+

``` source
var generationMarker: Data
```

## Discussion

When a content enumeration is underway, you must use the same `generationMarker` until the enumeration completes. If you restart content enumeration, you can use a new `generationMarker` value from that point onward.

## See Also

### Supporting paging

var offset: Int

An offset from the page’s generation marker.

static let initialPage: ContactItemPage

A static value the system uses to indicate the start of a new content enumeration.

