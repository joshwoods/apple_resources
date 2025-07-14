

- UIKit
- UITextInputTraits
-  enablesReturnKeyAutomatically 

Instance Property

# enablesReturnKeyAutomatically

A Boolean value that indicates whether the system automatically enables the Return key when the user enters text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var enablesReturnKeyAutomatically: Bool { get set }
```

## Discussion

The default value for this property is false. If you set it to true, the keyboard disables the Return key when the text entry area contains no text. As soon as the user enters some text, the Return key is automatically enabled.

## See Also

### Managing the keyboard behavior

var isSecureTextEntry: Bool

A Boolean value that indicates whether a text object disables copying, and in some cases, prevents recording/broadcasting and also hides the text.

