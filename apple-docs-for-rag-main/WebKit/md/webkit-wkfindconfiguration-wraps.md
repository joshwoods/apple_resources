

- WebKit
- WKFindConfiguration
-  wraps 

Instance Property

# wraps

A Boolean value that indicates whether the search wraps around to the other side of the page.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
var wraps: Bool { get set }
```

## Discussion

When the value of this property is true, the search wraps and continues at the other end of the page. For example, when a forward search reaches the bottom of the page, the search wraps back to the top of the page and continues. When a backward search reaches the top of the page, the search wraps back to the bottom of the page. The default value of this property is true.

## See Also

### Configuring the Search Parameters

var backwards: Bool

A Boolean value that indicates the search direction, relative to the current selection.

var caseSensitive: Bool

A Boolean value that indicates whether to consider case when matching the search string.

