

- TV Services
- TVContentItem
-  playURL Deprecated

Instance Property

# playURL

A URL that causes the app which created this content item to begin playing the item at the user’s current position.

tvOS 9.0–13.0Deprecated

``` source
var playURL: URL? { get set }
```

Deprecated

TVContentItem has been replaced by TVTopShelfItem

## Discussion

When the user presses play on the remote, opened, your application is launched if it wasn’t already running and then your UIApplication delegate is called. If at all possible, your application should immediately begin playing the content without any prompting for other information or displaying any other UI. Your app should start playback at the user’s current position within the content.

## See Also

### Inspecting the Application Launch Properties

var displayURL: URL?

A URL that causes the app which created this content item to display a description screen for the item.

Deprecated

