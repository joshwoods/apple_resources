

- Core Spotlight
- CSSearchableItemAttributeSet
-  containerOrder 

Instance Property

# containerOrder

The order of the item within the container.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var containerOrder: NSNumber? { get set }
```

## Discussion

For example, if the container represents a series of books, this property specifies the order in which the books should be read.

## See Also

### Describing containment

var containerDisplayName: String?

A localized string that specifies the name of a container to which the item belongs, suitable to display in the user interface.

var containerIdentifier: String?

The identifier of the container to which the item belongs.

var containerTitle: String?

The title of the container to which the item belongs.

