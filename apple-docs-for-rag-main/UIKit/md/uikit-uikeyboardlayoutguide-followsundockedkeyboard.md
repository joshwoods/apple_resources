

- UIKit
- UIKeyboardLayoutGuide
-  followsUndockedKeyboard 

Instance Property

# followsUndockedKeyboard

A Boolean value that determines if the layout guide tracks the keyboard when it’s undocked from the bottom of the screen.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var followsUndockedKeyboard: Bool { get set }
```

## Discussion

The default value is false; the guide tracks the keyboard only when docked. When the keyboard is off screen or undocked, the guide’s topAnchor matches the bottomAnchor of safeAreaLayoutGuide. To follow all keyboard anchors even when undocked or floating, set followsUndockedKeyboard to true.

