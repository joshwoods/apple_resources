

- UIKit
- UINavigationItem
-  largeTitleDisplayMode 

Instance Property

# largeTitleDisplayMode

The mode for displaying the title of the navigation bar.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var largeTitleDisplayMode: UINavigationItem.LargeTitleDisplayMode { get set }
```

## Discussion

When large titles are available, this property controls how the navigation bar displays the navigation item’s title. The default value of this property is UINavigationItem.LargeTitleDisplayMode.automatic, which causes the title to use the same styling as the previously displayed navigation item. You can change the value of this property to force the navigation bar to display a large title (UINavigationItem.LargeTitleDisplayMode.always) or a small title (UINavigationItem.LargeTitleDisplayMode.never) for this item.

If the prefersLargeTitles property of the navigation bar is false, this property has no effect and the navigation item’s title is always displayed as a small title.

## See Also

### Configuring the title

var title: String?

The navigation item’s title that displays in the navigation bar.

enum LargeTitleDisplayMode

Constants that indicate how to size the title of this item.

