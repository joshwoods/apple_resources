

- UIKit
- UIWebView
-  UIWebView.PaginationMode 

Enumeration

# UIWebView.PaginationMode

The layout of content in the web view, which determines the direction that the pages flow.

iOSiPadOS

``` source
enum PaginationMode
```

## Topics

### Constants

case unpaginated

Content appears as one long scrolling view with no distinct pages.

case leftToRight

Content is broken up into pages that flow from left to right.

case topToBottom

Content is broken up into pages that flow from top to bottom.

case bottomToTop

Content is broken up into pages that flow from bottom to top.

case rightToLeft

Content is broken up into pages that flow from right to left.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum NavigationType

Constant indicating the user’s action.

enum PaginationBreakingMode

The manner in which column- or page-breaking occurs.

struct UIDataDetectorTypes

Constants that define the types of information to detect in text-based content.

