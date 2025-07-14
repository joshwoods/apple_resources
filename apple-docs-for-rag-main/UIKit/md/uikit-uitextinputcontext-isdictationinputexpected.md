

- UIKit
- UITextInputContext
-  isDictationInputExpected 

Instance Property

# isDictationInputExpected

Returns a Boolean value that indicates whether someone is likely to use dictation to input text to the app.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+tvOS 16.4+visionOS 1.0+

``` source
var isDictationInputExpected: Bool { get set }
```

## Discussion

When dictation input is likely, adjust your UI or perform any actions you need to accommodate dictation input.

## See Also

### Getting the expected input type

var isHardwareKeyboardInputExpected: Bool

Returns a Boolean value that indicates whether someone is likely to enter text using a hardware keyboard.

var isPencilInputExpected: Bool

Returns a Boolean value that indicates whether someone is likely to use Apple Pencil for input.

