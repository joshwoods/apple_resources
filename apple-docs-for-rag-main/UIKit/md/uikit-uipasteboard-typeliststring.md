

- UIKit
- UIPasteboard
-  typeListString 

Type Property

# typeListString

An array of pasteboard-item representation types for string-type uniform type identifiers (UTIs), including the `kUTTypeUTF8PlainText` and `kUTTypeText` types. Related UIPasteboard properties are string and strings.

iOSiPadOSMac CatalystvisionOS

``` source
class var typeListString: NSArray
```

## See Also

### Constants

class var typeListURL: NSArray

An array of pasteboard-item representation types for URL-type uniform type identifiers (UTIs), including `kUTTypeURL`. Related UIPasteboard properties are url and urls.

class var typeListImage: NSArray

An array of pasteboard-item representation types for image-type uniform type identifiers (UTIs), including `kUTTypePNG` and `kUTTypeJPEG`. Related UIPasteboard properties are image and images.

class var typeListColor: NSArray

An array of pasteboard-item representation types for colors. Related UIPasteboard properties are color and colors.

class let typeAutomatic: String

An array of pasteboard-item representation types with automatically-determined uniform type identifiers (UTIs).

