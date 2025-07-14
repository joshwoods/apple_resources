

- UIKit
- UIPasteboard
-  urls 

Instance Property

# urls

An array of URL objects in all pasteboard items.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var urls: [URL]? { get set }
```

## Discussion

The value stored in this property is an array of NSURL objects. The associated array of representation types is typeListURL, which includes type `kUTTypeURL`. Setting this property replaces all current items in the pasteboard with the new items. The returned array may have fewer objects than the number of pasteboard items; this happens if a pasteboard item does not have a value of the indicated type.

Note

Do not use this property to determine if a pasteboard contains URL data. Instead, use the hasURLs property.

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

var color: UIColor?

The color object of the first pasteboard item.

var colors: [UIColor]?

An array of color objects in all pasteboard items.

