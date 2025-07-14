

- UIKit
- UIContextualAction
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the action button.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying @MainActor
var backgroundColor: UIColor! { get set }
```

## Discussion

The default value of this property is determined by the value of the style property, which determines the default appearance of the button. Assigning a new color to this property changes the background to the color that you specify.

## See Also

### Configuring the appearance

var title: String?

The title displayed on the action button.

var image: UIImage?

The image to display in the action button.

