

- WebKit
-  WebNavigationType Deprecated

Enumeration

# WebNavigationType

Possible values for the WebActionNavigationTypeKey key that appears in an action dictionary.

macOS 10.3–10.14Deprecated

``` source
enum WebNavigationType
```

## Topics

### Constants

case linkClicked

A link (an `href`) was clicked.

case formSubmitted

A form was submitted.

case backForward

The user clicked back or forward button.

case reload

The user hit the reload button.

case formResubmitted

A form was resubmitted (through a back, forward or reload action).

case other

Navigation is taking place for some other reason.

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

### Content

enum WebViewInsertAction

The type of user action that initiated a delegate message.

Deprecated

