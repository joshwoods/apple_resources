

- UIKit
- UIMenuElement
-  image 

Instance Property

# image

The image to display alongside the menu element’s title.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var image: UIImage? { get }
```

## Discussion

Only the context menu system supports the display of an image, and only when the app is running in iOS.

## See Also

### Getting the element attributes

var title: String

The title of the menu element.

var subtitle: String?

The subtitle to display alongside the menu element’s title.

