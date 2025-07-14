

- UIKit
- UIResponder
-  keyboardWillHideNotification 

Type Property

# keyboardWillHideNotification

A notification that posts immediately prior to dismissing the keyboard.

iOSiPadOSMac CatalystvisionOS

``` source
nonisolated
class let keyboardWillHideNotification: NSNotification.Name
```

## Discussion

In iOS 16.1 and later, the notification object is the UIScreen that the keyboard appears on. In earlier versions of iOS, the notification object is `nil`.

The `userInfo` dictionary contains information about the keyboard. To get the location and size of the keyboard from the `userInfo` dictionary, use keyboardFrameBeginUserInfoKey and keyboardFrameEndUserInfoKey.

The keyboard’s frame uses the screen’s coordinate space, which is different than the coordinate space of your views. Although they might sometimes match, such as when your app is full screen, they might be different when your app isn’t full screen, such as in Split View, Slide Over, and Stage Manager. This means you need to account for this difference by converting the keyboard’s frame from the screen’s coordinate space to that of your views. For an example of how to handle this conversion, see keyboardFrameEndUserInfoKey.

The system posts this notification on the main actor. An app running in visionOS never receives this notification. The system displays the keyboard in a separate window, leaving the app’s window unaffected by the keyboard’s appearance and disappearance.

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

class let keyboardIsLocalUserInfoKey: String

A user info key to retrieve a Boolean value that indicates whether the keyboard belongs to the current app.

class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

