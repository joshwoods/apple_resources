

- UIKit
- UIResponder
-  keyboardIsLocalUserInfoKey 

Type Property

# keyboardIsLocalUserInfoKey

A user info key to retrieve a Boolean value that indicates whether the keyboard belongs to the current app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
nonisolated
class let keyboardIsLocalUserInfoKey: String
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value that indicates whether the keyboard belongs to the current app. With Multitasking in iPadOS, the system notifies all visible apps when the keyboard appears and disappears. The value is true for the app that caused the keyboard to appear and false for the other apps.

## See Also

### Constants

class let keyboardAnimationCurveUserInfoKey: String

A user info key to retrieve the animation curve that the system uses to animate the keyboard onto or off the screen.

class let keyboardAnimationDurationUserInfoKey: String

A user info key to retrieve the duration of the keyboard animation in seconds.

class let keyboardDidChangeFrameNotification: NSNotification.Name

A notification that posts immediately after a change in the keyboard’s frame.

class let keyboardDidHideNotification: NSNotification.Name

A notification that posts immediately after dismissing the keyboard.

class let keyboardDidShowNotification: NSNotification.Name

A notification that posts immediately after displaying the keyboard.

class let keyboardFrameBeginUserInfoKey: String

A user info key to retrieve the keyboard’s frame at the beginning of its animation.

class let keyboardFrameEndUserInfoKey: String

A user info key to retrieve the keyboard’s frame at the end of its animation.

class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

class let keyboardWillHideNotification: NSNotification.Name

A notification that posts immediately prior to dismissing the keyboard.

class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

