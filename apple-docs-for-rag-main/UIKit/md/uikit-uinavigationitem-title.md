

- UIKit
- UINavigationItem
-  title 

Instance Property

# title

The navigation item’s title that displays in the navigation bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var title: String? { get set }
```

## Discussion

The default value is `nil`.

When the navigation item is on the navigation item stack and is second from the top — in other words, its view controller manages the views that the user would navigate back to — the value in this property is used for the back button on the top-most navigation bar. If the value of this property is `nil`, the system uses the string “Back” as the text of the back button. In iOS 11 and later, the size and position of the title is determined by the prefersLargeTitles property of the navigation bar and the largeTitleDisplayMode property of the navigation item.

## See Also

### Related Documentation

init(title: String)

Creates a navigation item with the specified title.

var titleView: UIView?

A custom view that displays in the center of the navigation bar when the receiver is the top item.

class UINavigationItem

The items that a navigation bar displays when the associated view controller is visible.

### Configuring the title

var largeTitleDisplayMode: UINavigationItem.LargeTitleDisplayMode

The mode for displaying the title of the navigation bar.

enum LargeTitleDisplayMode

Constants that indicate how to size the title of this item.

