

- UIKit
- UIPrintInteractionController
-  printingItems 

Instance Property

# printingItems

An array of ready-to-print objects.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printingItems: [Any]? { get set }
```

## Discussion

The array must contain NSURL, NSData, UIImage, or ALAsset objects in any combination. Objects of the first two types must reference or contain image data or PDF data. `NSURL` objects must use the `file:` or `assets-library:` scheme or any scheme that can return an NSData object with a registered protocol. Image data (including that encapsulated by UIImage and ALAsset objects) must be in a format supported by the Image I/O framework; see UIImage for more information. An ALAsset object must be of type ALAssetTypePhoto. Items are printed in array-index order. The array is released at the end of the print job. The default value is `nil`.

If you set this property, `UIPrintInteractionController` sets the printingItem, printPageRenderer, and printFormatter properties to `nil`. (Only one of these properties can be set for a print job.)

If this property is set, the printing options do not include the control for selecting a page range, even if the showsPageRange property is set to true. If you want page-range selection, you should use the printingItem property instead.

## See Also

### Providing the source of printable content

var printingItem: Any?

A single ready-to-print object.

var printPageRenderer: UIPrintPageRenderer?

An object that draws pages of printable content when UIKit requests it.

var printFormatter: UIPrintFormatter?

An object that lays out the content of pages according to the kind of content.

