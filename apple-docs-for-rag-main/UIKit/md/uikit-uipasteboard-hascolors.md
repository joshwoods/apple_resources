

- UIKit
- UIPasteboard
-  hasColors 

Instance Property

# hasColors

A Boolean value that indicates whether the pasteboard contains contains a nonempty array of colors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var hasColors: Bool { get }
```

## Discussion

Employ this property to determine if a pasteboard contains color data.

Do not use the color or colors properties to determine whether a pasteboard contains color data, because doing so consumes resources needlessly.

## See Also

### Checking for data types on a pasteboard

var hasImages: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of images.

var hasStrings: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of strings.

var hasURLs: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of URLs.

