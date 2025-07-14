

- CarPlay
- CPTemplate
-  tabTitle 

Instance Property

# tabTitle

A short title that describes the content of the tab.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var tabTitle: String? { get set }
```

## Discussion

CarPlay only uses the title when the template is a root-template of a tab bar, otherwise setting this property has no effect.

## See Also

### Accessing Tab Information

var tabImage: UIImage?

An image that represents the content of the tab.

var tabSystemItem: UITabBarItem.SystemItem

A system object that provides a title and image for common tab content, such as contacts or favorites.

var showsTabBadge: Bool

An indicator you use to call attention to the tab.

