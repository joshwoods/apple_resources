

- CarPlay
- CPTemplate
-  tabImage 

Instance Property

# tabImage

An image that represents the content of the tab.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var tabImage: UIImage? { get set }
```

## Discussion

This image has precedence over any system item that tabSystemItem specifies, and CarPlay only uses it when the template is a root-template of a tab bar.

## See Also

### Accessing Tab Information

var tabTitle: String?

A short title that describes the content of the tab.

var tabSystemItem: UITabBarItem.SystemItem

A system object that provides a title and image for common tab content, such as contacts or favorites.

var showsTabBadge: Bool

An indicator you use to call attention to the tab.

