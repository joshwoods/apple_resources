

- ContactProvider
- ContactItemPage
-  offset 

Instance Property

# offset

An offset from the page’s generation marker.

iOS 18.0+iPadOS 18.0+

``` source
var offset: Int
```

## Discussion

You can use the offset to track a contiguous number of contact items which have been successfully enumerated for that database generation.

## See Also

### Supporting paging

var generationMarker: Data

A value specific to your data source identifying the database generation when enumeration of content started.

static let initialPage: ContactItemPage

A static value the system uses to indicate the start of a new content enumeration.

