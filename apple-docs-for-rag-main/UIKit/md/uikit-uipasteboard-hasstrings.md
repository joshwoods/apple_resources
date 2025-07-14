

- UIKit
- UIPasteboard
-  hasStrings 

Instance Property

# hasStrings

A Boolean value that indicates whether the pasteboard contains a nonempty array of strings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var hasStrings: Bool { get }
```

## Discussion

Employ this property to determine if a pasteboard contains string data.

Do not use the string or strings properties to determine whether a pasteboard contains string data, because doing so consumes resources needlessly.

## See Also

### Checking for data types on a pasteboard

var hasColors: Bool

A Boolean value that indicates whether the pasteboard contains contains a nonempty array of colors.

var hasImages: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of images.

var hasURLs: Bool

A Boolean value that indicates whether the pasteboard contains a nonempty array of URLs.

