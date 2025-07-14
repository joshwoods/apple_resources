

- UIKit
- UIScrollView
-  UIScrollView.KeyboardDismissMode 

Enumeration

# UIScrollView.KeyboardDismissMode

Constants that determine how the system dismisses the keyboard when a drag begins in the scroll view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS

``` source
enum KeyboardDismissMode
```

## Overview

You use these constants to set the value of the keyboardDismissMode property.

## Topics

### Constants

case none

A mode in which a drag doesn’t dismiss the keyboard.

case onDrag

A mode in which the keyboard dismisses when a drag begins.

case interactive

A mode in which the keyboard follows the dragging touch offscreen, and can be pulled upward again to cancel the dismiss.

case onDragWithAccessory

A mode in which the keyboard and accessory view dismiss together when a drag begins.

case interactiveWithAccessory

A mode in which the keyboard and accessory view both follow the dragging touch offscreen, and can be pulled upward again to cancel the dismiss.

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

### Dismissing the keyboard

var keyboardDismissMode: UIScrollView.KeyboardDismissMode

The manner in which the system dismisses the keyboard when a drag begins in the scroll view.

