

- UIKit
- UITextInput
-  textInputView 

Instance Property

# textInputView

An affiliated view that provides a coordinate system for all geometric values in the protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional var textInputView: UIView { get }
```

## Discussion

The view that both draws the text and provides a coordinate system for all geometric values in this protocol. (This is typically an instance of the UITextInput-adopting class.) If this property is unimplemented, the first view in the responder chain is selected.

