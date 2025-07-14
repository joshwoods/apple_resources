

- WebKit
- WKWebExtension
-  WKWebExtension.WindowState 

Enumeration

# WKWebExtension.WindowState

Constants used by WKWebExtensionWindow to indicate possible states of a window.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
enum WindowState
```

## Topics

### Enumeration Cases

case fullscreen

Indicates a window is in full-screen mode.

case maximized

Indicates a window is maximized.

case minimized

Indicates a window is minimized.

case normal

Indicates a window is in its normal state.

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

### Enumerations

enum WindowType

Constants used by WKWebExtensionWindow to indicate the type of a window.

