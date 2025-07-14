

- UIKit
- UITextInputContext
-  isHardwareKeyboardInputExpected 

Instance Property

# isHardwareKeyboardInputExpected

Returns a Boolean value that indicates whether someone is likely to enter text using a hardware keyboard.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+tvOS 16.4+visionOS 1.0+

``` source
var isHardwareKeyboardInputExpected: Bool { get set }
```

## Discussion

When hardware keyboard input is likely, adjust your UI or perform any actions you need to accommodate that input.

## See Also

### Getting the expected input type

var isDictationInputExpected: Bool

Returns a Boolean value that indicates whether someone is likely to use dictation to input text to the app.

var isPencilInputExpected: Bool

Returns a Boolean value that indicates whether someone is likely to use Apple Pencil for input.

