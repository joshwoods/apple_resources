

- UIKit
- UIPasteboard
-  hasURLs 

Instance Property

# hasURLs

A Boolean value that indicates whether the pasteboard contains a nonempty array of URLs.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var hasURLs: Bool { get }
```

## Discussion

Employ this property to determine if a pasteboard contains URL data.

Do not use the url or urls properties to determine whether a pasteboard contains URL data, because doing so consumes resources needlessly.

## See Also

### Checking for data types on a pasteboard

var hasColors: Bool

A Boolean value that indicates whether the pasteboard contains contains a nonempty array of colors.

var hasImages: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of images.

var hasStrings: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of strings.

