

- UIKit
- UIResponder
-  keyboardAnimationDurationUserInfoKey 

Type Property

# keyboardAnimationDurationUserInfoKey

A user info key to retrieve the duration of the keyboard animation in seconds.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
nonisolated
class let keyboardAnimationDurationUserInfoKey: String
```

## Discussion

The value for this key is an NSNumber object containing a `double` that represents the duration of the keyboard animation in seconds. You can use this value to match the animation of the keyboard in your own animations.

For an example of how to match the keyboard’s animation, see keyboardAnimationCurveUserInfoKey.

## See Also

### Constants

class let keyboardAnimationCurveUserInfoKey: String

A user info key to retrieve the animation curve that the system uses to animate the keyboard onto or off the screen.

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

class let keyboardIsLocalUserInfoKey: String

A user info key to retrieve a Boolean value that indicates whether the keyboard belongs to the current app.

class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

class let keyboardWillHideNotification: NSNotification.Name

A notification that posts immediately prior to dismissing the keyboard.

class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

