

- UIKit
- UIResponder
-  keyboardAnimationCurveUserInfoKey 

Type Property

# keyboardAnimationCurveUserInfoKey

A user info key to retrieve the animation curve that the system uses to animate the keyboard onto or off the screen.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
nonisolated
class let keyboardAnimationCurveUserInfoKey: String
```

## Discussion

The value for this key is an NSNumber object that contains a UIView.AnimationCurve constant used to determine how the system animates the keyboard onto or off the screen. You can use this value to match the animation of the keyboard in your own animations.

Before using this value, convert the animation curve constant to UIView.AnimationOptions, which you can pass to one of UIKit’s animation methods, such as animate(withDuration:animations:completion:).

- Swift
- Objective-C

```
// Get the animation curve constant and the duration for your animation.
guard let animationCurve = userInfo[UIResponder.keyboardAnimationCurveUserInfoKey] as? UInt,
      let animationDuration = userInfo[UIResponder.keyboardAnimationDurationUserInfoKey] as? Double else { return }

// Convert the animation curve constant to animation options.
let animationOptions = UIView.AnimationOptions(rawValue: animationCurve 

```
// Convert the animation curve constant to animation options.
UIViewAnimationOptions options = (UIViewAnimationOptions)[[userInfo objectForKey:UIKeyboardAnimationCurveUserInfoKey]
                          integerValue] 

## See Also

### Constants

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

class let keyboardIsLocalUserInfoKey: String

A user info key to retrieve a Boolean value that indicates whether the keyboard belongs to the current app.

class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

class let keyboardWillHideNotification: NSNotification.Name

A notification that posts immediately prior to dismissing the keyboard.

class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

