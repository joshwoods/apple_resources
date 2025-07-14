

- AppKit
- NSDraggingItemEnumerationOptions
-  clearNonenumeratedImages 

Type Property

# clearNonenumeratedImages

A constant that indicates the enumeration clears the image components provider for all dragging items that don’t meet the classes and search options criteria.

macOS 10.7+

``` source
static var clearNonenumeratedImages: NSDraggingItemEnumerationOptions { get }
```

## Discussion

Specify this option when you enumerate dragging items to hide the drag image for nonvalid items for this destination. The enumeration sets the imageComponentsProvider to `nil` for all dragging items that don’t meet the classes and search options criteria.

## See Also

### Constants

static var concurrent: NSDraggingItemEnumerationOptions

A constant that indicates the enumeration processes dragging items concurrently.

