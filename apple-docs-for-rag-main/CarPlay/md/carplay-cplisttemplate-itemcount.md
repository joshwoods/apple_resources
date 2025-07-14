

- CarPlay
- CPListTemplate
-  itemCount 

Instance Property

# itemCount

The total number of items, across all sections, in the list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var itemCount: Int { get }
```

## Discussion

This value never exceeds maximumItemCount. If you initialize a list where the total number of items, across all sections, is greater than maximumItemCount, CarPlay only displays items up to this limit and discards the rest.

## See Also

### Getting Supplementary Information

class var maximumItemCount: Int

The maximum number of items, across all sections, that the template can display.

func indexPath(for: any CPListTemplateItem) -> IndexPath?

Returns the index path for the specified item.

var title: String?

The title that the navigation bar displays when the template is visible.

