

- UIKit
- UIInputView
-  UIInputView.Style 

Enumeration

# UIInputView.Style

Constants that indicate the appearance changes for an input view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum Style
```

## Topics

### Constants

case `default`

Apply blur behaviors to the view so that it looks like it belongs with the keyboard.

case keyboard

Apply both blur and tinting effects to the view to mimic the keyboard background.

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

### Getting the input style

var inputViewStyle: UIInputView.Style

The style for the content of the view.

