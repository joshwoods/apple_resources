

- UIKit
- UITextInputTraits
-  isSecureTextEntry 

Instance Property

# isSecureTextEntry

A Boolean value that indicates whether a text object disables copying, and in some cases, prevents recording/broadcasting and also hides the text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var isSecureTextEntry: Bool { get set }
```

## Discussion

This property is set to false by default. Setting this property to true in any view that conforms to UITextInputTraits disables the user’s ability to copy the text in the view and, in some cases, also disables the user’s ability to record and broadcast the text in the view.

Setting this property to true in a UITextField object additionally enables a password-style experience, in which the text being entered is obscured.

## See Also

### Managing the keyboard behavior

var enablesReturnKeyAutomatically: Bool

A Boolean value that indicates whether the system automatically enables the Return key when the user enters text.

