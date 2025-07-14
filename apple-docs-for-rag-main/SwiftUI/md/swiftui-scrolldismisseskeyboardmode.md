

- SwiftUI
-  ScrollDismissesKeyboardMode 

Structure

# ScrollDismissesKeyboardMode

The ways that scrollable content can interact with the software keyboard.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
struct ScrollDismissesKeyboardMode
```

## Overview

Use this type in a call to the scrollDismissesKeyboard(_:) modifier to specify the dismissal behavior of scrollable views.

## Topics

### Getting modes

static var automatic: ScrollDismissesKeyboardMode

Determine the mode automatically based on the surrounding context.

static var immediately: ScrollDismissesKeyboardMode

Dismiss the keyboard as soon as scrolling starts.

static var interactively: ScrollDismissesKeyboardMode

Enable people to interactively dismiss the keyboard as part of the scroll operation.

static var never: ScrollDismissesKeyboardMode

Never dismiss the keyboard automatically as a result of scrolling.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Interacting with a software keyboard

func scrollDismissesKeyboard(ScrollDismissesKeyboardMode) -> some View

Configures the behavior in which scrollable content interacts with the software keyboard.

var scrollDismissesKeyboardMode: ScrollDismissesKeyboardMode

The way that scrollable content interacts with the software keyboard.

