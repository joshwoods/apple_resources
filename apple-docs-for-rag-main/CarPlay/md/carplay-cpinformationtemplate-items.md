

- CarPlay
- CPInformationTemplate
-  items 

Instance Property

# items

The items that the template displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var items: [CPInformationItem] { get set }
```

## Discussion

Assign a new array to this property to update the items that the template displays. The template can display 10 items maximum. If the array contains more items, the template uses only the first 10.

## See Also

### Managing the Items

class CPInformationItem

A data object that provides content for an information template.

class CPInformationRatingItem

A data object that provides rated content for an information template.

