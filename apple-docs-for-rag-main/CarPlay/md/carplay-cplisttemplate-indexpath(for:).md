

- CarPlay
- CPListTemplate
-  indexPath(for:) 

Instance Method

# indexPath(for:)

Returns the index path for the specified item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func indexPath(for item: any CPListTemplateItem) -> IndexPath?
```

## Parameters 

`item`  

The item to find in the list.

## Return Value

The item’s index path in the list, or nil if the list doesn’t contain the item.

## See Also

### Getting Supplementary Information

class var maximumItemCount: Int

The maximum number of items, across all sections, that the template can display.

var itemCount: Int

The total number of items, across all sections, in the list.

var title: String?

The title that the navigation bar displays when the template is visible.

