

- CarPlay
- CPTemplate
-  showsTabBadge 

Instance Property

# showsTabBadge

An indicator you use to call attention to the tab.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var showsTabBadge: Bool { get set }
```

## Discussion

Set this property to `true` to display a small red indicator on the tab to show that it requires action from the user, or is displaying ephemeral information.

CarPlay only displays the indicator when the template is a root-template of a tab bar, otherwise setting this property has no effect.

## See Also

### Accessing Tab Information

var tabTitle: String?

A short title that describes the content of the tab.

var tabImage: UIImage?

An image that represents the content of the tab.

var tabSystemItem: UITabBarItem.SystemItem

A system object that provides a title and image for common tab content, such as contacts or favorites.

