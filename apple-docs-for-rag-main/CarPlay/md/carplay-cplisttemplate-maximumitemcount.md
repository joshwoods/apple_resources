

- CarPlay
- CPListTemplate
-  maximumItemCount 

Type Property

# maximumItemCount

The maximum number of items, across all sections, that the template can display.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class var maximumItemCount: Int { get }
```

## Discussion

This property’s value is dependent on any user interface limits that the vehicle imposes. See CPSessionConfiguration for more information. At runtime, use this value to determine the maximum number of items, across all sections, that your list can display.

## See Also

### Getting Supplementary Information

var itemCount: Int

The total number of items, across all sections, in the list.

func indexPath(for: any CPListTemplateItem) -> IndexPath?

Returns the index path for the specified item.

var title: String?

The title that the navigation bar displays when the template is visible.

