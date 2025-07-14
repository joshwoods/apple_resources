

- UIKit
- UIPasteboard
-  typeAutomatic 

Type Property

# typeAutomatic

An array of pasteboard-item representation types with automatically-determined uniform type identifiers (UTIs).

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class let typeAutomatic: String
```

## Discussion

Use this type in the setItems(_:options:) method to automatically insert appropriate UTIs for supported types. In iOS 10, supported types are NSString, NSAttributedString, NSURL, UIImage, and UIColor.

## See Also

### Constants

class var typeListString: NSArray

An array of pasteboard-item representation types for string-type uniform type identifiers (UTIs), including the `kUTTypeUTF8PlainText` and `kUTTypeText` types. Related UIPasteboard properties are string and strings.

class var typeListURL: NSArray

An array of pasteboard-item representation types for URL-type uniform type identifiers (UTIs), including `kUTTypeURL`. Related UIPasteboard properties are url and urls.

class var typeListImage: NSArray

An array of pasteboard-item representation types for image-type uniform type identifiers (UTIs), including `kUTTypePNG` and `kUTTypeJPEG`. Related UIPasteboard properties are image and images.

class var typeListColor: NSArray

An array of pasteboard-item representation types for colors. Related UIPasteboard properties are color and colors.

