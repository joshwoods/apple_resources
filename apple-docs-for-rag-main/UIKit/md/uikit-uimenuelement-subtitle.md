

- UIKit
- UIMenuElement
-  subtitle 

Instance Property

# subtitle

The subtitle to display alongside the menu element’s title.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var subtitle: String? { get set }
```

## Discussion

Only the context menu system supports the display of a subtitle, and only when the app is running on iOS.

## See Also

### Getting the element attributes

var title: String

The title of the menu element.

var image: UIImage?

The image to display alongside the menu element’s title.

