

- UIKit
- UIWebView
-  UIWebView.NavigationType 

Enumeration

# UIWebView.NavigationType

Constant indicating the user’s action.

iOSiPadOS

``` source
enum NavigationType
```

## Topics

### Constants

case linkClicked

User tapped a link.

case formSubmitted

User submitted a form.

case backForward

User tapped the back or forward button.

case reload

User tapped the reload button.

case formResubmitted

User resubmitted a form.

case other

Some other action occurred.

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

enum PaginationBreakingMode

The manner in which column- or page-breaking occurs.

enum PaginationMode

The layout of content in the web view, which determines the direction that the pages flow.

struct UIDataDetectorTypes

Constants that define the types of information to detect in text-based content.

