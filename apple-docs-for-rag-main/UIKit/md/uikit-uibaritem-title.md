

- UIKit
- UIBarItem
-  title 

Instance Property

# title

The title displayed on the item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var title: String? { get set }
```

## Discussion

You should set this property before adding the item to a bar. The default value is `nil`.

## See Also

### Getting and setting properties

var image: UIImage?

The image used to represent the item.

var landscapeImagePhone: UIImage?

The image to use to represent the item in landscape orientation when using the iPhone appearance idiom.

var largeContentSizeImage: UIImage?

The image to display for users who are blind or have low vision.

var imageInsets: UIEdgeInsets

The image inset or outset for each edge.

var landscapeImagePhoneInsets: UIEdgeInsets

The image inset or outset for each edge of the image in landscape orientation when using the iPhone appearance idiom.

var largeContentSizeImageInsets: UIEdgeInsets

The insets to apply to the bar item’s large image when displaying the image in an assistive UI.

var isEnabled: Bool

A Boolean value indicating whether the item is enabled.

var tag: Int

The bar item’s tag, an app-supplied integer that you can use to identify bar item objects in your app.

