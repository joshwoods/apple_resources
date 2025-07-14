

- UIKit
- UIPasteboard
-  hasImages 

Instance Property

# hasImages

A Boolean value that indicates whether the pasteboard contains a nonempty array of images.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var hasImages: Bool { get }
```

## Discussion

Employ this property to determine if a pasteboard contains image data.

Do not use the image or images properties to determine whether a pasteboard contains image data, because doing so consumes resources needlessly.

## See Also

### Checking for data types on a pasteboard

var hasColors: Bool

A Boolean value that indicates whether the pasteboard contains contains a nonempty array of colors.

var hasStrings: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of strings.

var hasURLs: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of URLs.

