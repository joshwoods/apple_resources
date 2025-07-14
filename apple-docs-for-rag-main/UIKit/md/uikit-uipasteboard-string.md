

- UIKit
- UIPasteboard
-  string 

Instance Property

# string

The string value of the first pasteboard item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var string: String? { get set }
```

## Discussion

The value stored in this property is an NSString object. The associated array of representation types is typeListString, which includes type `kUTTypeUTF8PlainText`. Setting this property replaces all current items in the pasteboard with the new item. If the first item has no value of the indicated type, `nil` is returned.

Note

Do not use this property to determine if a pasteboard contains string data. Instead, use the hasStrings property.

## See Also

### Getting and setting pasteboard items of standard data types

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

var color: UIColor?

The color object of the first pasteboard item.

var colors: [UIColor]?

An array of color objects in all pasteboard items.

