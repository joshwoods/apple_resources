

- TV Services
- TVContentItem
-  displayURL Deprecated

Instance Property

# displayURL

A URL that causes the app which created this content item to display a description screen for the item.

tvOS 9.0–13.0Deprecated

``` source
var displayURL: URL? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

When the user selects the item, your application is launched if it wasn’t already running and then your UIApplication delegate is called. If at all possible, your application should immediately display the description of the item without any prompting for other information or displaying any other UI.

## See Also

### Inspecting the Application Launch Properties

var playURL: URL?

A URL that causes the app which created this content item to begin playing the item at the user’s current position.

Deprecated

