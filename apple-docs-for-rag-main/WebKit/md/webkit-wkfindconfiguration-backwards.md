

- WebKit
- WKFindConfiguration
-  backwards 

Instance Property

# backwards

A Boolean value that indicates the search direction, relative to the current selection.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS 1.0+

``` source
@MainActor
var backwards: Bool { get set }
```

## Discussion

When the value of this property is true, searches proceed backward from the current selection. When the value is false, searches proceed forward from the current selection. The default value of this property is false.

The web view respects the writing direction of its content. For example, a forward search moves right-to-left and top-to-bottom for a right-to-left language.

## See Also

### Configuring the Search Parameters

var caseSensitive: Bool

A Boolean value that indicates whether to consider case when matching the search string.

var wraps: Bool

A Boolean value that indicates whether the search wraps around to the other side of the page.

