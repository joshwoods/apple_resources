

- SwiftUI
- EnvironmentValues
-  scrollDismissesKeyboardMode 

Instance Property

# scrollDismissesKeyboardMode

The way that scrollable content interacts with the software keyboard.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
var scrollDismissesKeyboardMode: ScrollDismissesKeyboardMode { get set }
```

## Discussion

The default value is automatic. Use the scrollDismissesKeyboard(_:) modifier to configure this property.

## See Also

### Interacting with a software keyboard

func scrollDismissesKeyboard(ScrollDismissesKeyboardMode) -> some View

Configures the behavior in which scrollable content interacts with the software keyboard.

struct ScrollDismissesKeyboardMode

The ways that scrollable content can interact with the software keyboard.

