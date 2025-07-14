

- UIKit
- UITextInput
-  inputDelegate 

Instance Property

# inputDelegate

An input delegate that receives a notification when text changes or when the selection changes.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
weak var inputDelegate: (any UITextInputDelegate)? { get set }
```

**Required**

## Discussion

The text input system automatically assigns a delegate to this property at runtime. It is the responsibility of the view that adopts the UITextInput protocol to notify the input delegate at the appropriate junctures.

## See Also

### Handling text input

protocol UITextInputDelegate

An intermediary between a document and the text input system.

