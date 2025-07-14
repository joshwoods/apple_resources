

- CarPlay
- CPTemplate
-  tabSystemItem 

Instance Property

# tabSystemItem

A system object that provides a title and image for common tab content, such as contacts or favorites.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var tabSystemItem: UITabBarItem.SystemItem { get set }
```

## Discussion

You should specify either a system item, or a tab title and tab image. The tab image has precedence over the system item if both properties are set.

CarPlay only uses this value when the template is a root-template of a tab bar.

## See Also

### Accessing Tab Information

var tabTitle: String?

A short title that describes the content of the tab.

var tabImage: UIImage?

An image that represents the content of the tab.

var showsTabBadge: Bool

An indicator you use to call attention to the tab.

