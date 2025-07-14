

- UIKit
- UIPasteboard
-  color 

Instance Property

# color

The color object of the first pasteboard item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying
var color: UIColor? { get set }
```

## Discussion

The value stored in this property is a UIColor object. The associated array of representation types is typeListColor. Setting this property replaces all current items in the pasteboard with the new item. If the first item has no value of the indicated type, `nil` is returned.

Note

Do not use this property to determine if a pasteboard contains color data. Instead, use the hasColors property.

## See Also

### Getting and setting pasteboard items of standard data types

var string: String?

The string value of the first pasteboard item.

var strings: [String]?

An array of strings in all pasteboard items.

var image: UIImage?

The image object of the first pasteboard item.

var images: [UIImage]?

An array of image objects in all pasteboard items.

var url: URL?

The URL object of the first pasteboard item.

var urls: [URL]?

An array of URL objects in all pasteboard items.

var colors: [UIColor]?

An array of color objects in all pasteboard items.

