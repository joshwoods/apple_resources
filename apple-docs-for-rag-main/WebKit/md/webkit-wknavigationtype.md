

- WebKit
-  WKNavigationType 

Enumeration

# WKNavigationType

The type of action that triggered the navigation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
enum WKNavigationType
```

## Topics

### Getting the Navigation Types

case linkActivated

A link activation.

case formSubmitted

A request to submit a form.

case backForward

A request for the frame’s next or previous item.

case reload

A request to reload the webpage.

case formResubmitted

A request to resubmit a form.

case other

A navigation request that originates for some other reason.

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

### Getting the navigation type

var navigationType: WKNavigationType

The type of action that triggered the navigation.

