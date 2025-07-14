

- UIKit
- UILargeContentViewerItem
-  scalesLargeContentImage 

Instance Property

# scalesLargeContentImage

A Boolean value that indicates whether the view scales the item’s image to a larger size or not.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var scalesLargeContentImage: Bool { get }
```

**Required**

## Discussion

If false, the viewer displays the image at its intrinsic size.

Tip

For best results when scaling, use a PDF asset with the Preserve Vector Data checked in the asset catalog.

## See Also

### Configuring display properties

var largeContentTitle: String?

A string that describes an item to display in the large content viewer.

**Required**

var largeContentImage: UIImage?

An image that represents an item to display in the large content viewer.

**Required**

var largeContentImageInsets: UIEdgeInsets

Insets to adjust the position of the item’s image so it appears visually centered in the large content viewer.

**Required**

