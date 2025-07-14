

- Core Spotlight
- CSSearchableItemAttributeSet
-  containerDisplayName 

Instance Property

# containerDisplayName

A localized string that specifies the name of a container to which the item belongs, suitable to display in the user interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var containerDisplayName: String? { get set }
```

## Discussion

For example, a container display name might be the title of a series of books. When you specify the containment properties, Spotlight can treat individual items as part of an ordered set.

## See Also

### Describing containment

var containerIdentifier: String?

The identifier of the container to which the item belongs.

var containerOrder: NSNumber?

The order of the item within the container.

var containerTitle: String?

The title of the container to which the item belongs.

