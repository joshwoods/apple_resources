

- UIKit
- UIBarItem
-  largeContentSizeImageInsets 

Instance Property

# largeContentSizeImageInsets

The insets to apply to the bar item’s large image when displaying the image in an assistive UI.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var largeContentSizeImageInsets: UIEdgeInsets { get set }
```

## Discussion

The default value of this property is zero.

## See Also

### Getting and setting properties

var title: String?

The title displayed on the item.

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

var isEnabled: Bool

A Boolean value indicating whether the item is enabled.

var tag: Int

The bar item’s tag, an app-supplied integer that you can use to identify bar item objects in your app.

