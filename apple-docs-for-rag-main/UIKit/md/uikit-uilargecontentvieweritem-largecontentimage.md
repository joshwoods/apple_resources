

- UIKit
- UILargeContentViewerItem
-  largeContentImage 

Instance Property

# largeContentImage

An image that represents an item to display in the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var largeContentImage: UIImage? { get }
```

**Required**

## Discussion

To present content in the large content viewer, you can provide either largeContentTitle or largeContentImage, or both.

This property defaults to an appropriate value for UIKit classes, otherwise `nil`.

## See Also

### Configuring display properties

var largeContentTitle: String?

A string that describes an item to display in the large content viewer.

**Required**

var largeContentImageInsets: UIEdgeInsets

Insets to adjust the position of the item’s image so it appears visually centered in the large content viewer.

**Required**

var scalesLargeContentImage: Bool

A Boolean value that indicates whether the view scales the item’s image to a larger size or not.

**Required**

