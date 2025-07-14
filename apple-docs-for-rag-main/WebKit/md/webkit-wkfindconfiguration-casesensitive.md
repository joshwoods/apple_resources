

- WebKit
- WKFindConfiguration
-  caseSensitive 

Instance Property

# caseSensitive

A Boolean value that indicates whether to consider case when matching the search string.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
var caseSensitive: Bool { get set }
```

## Discussion

When the value of this property is true, the web view takes case into account when matching the search string. The default value of this property is false.

## See Also

### Configuring the Search Parameters

var backwards: Bool

A Boolean value that indicates the search direction, relative to the current selection.

var wraps: Bool

A Boolean value that indicates whether the search wraps around to the other side of the page.

