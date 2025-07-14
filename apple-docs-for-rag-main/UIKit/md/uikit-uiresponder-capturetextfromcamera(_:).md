

- UIKit
- UIResponder
-  captureTextFromCamera(\_:) 

Instance Method

# captureTextFromCamera(\_:)

Starts scanning text using the device’s camera.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
func captureTextFromCamera(_ sender: Any?)
```

## Parameters 

`sender`  

The object that invokes this method.

## Discussion

To receive callbacks from the data scanner, the responder should conform to either the UIKeyInput or UITextInput protocol. If it conforms to UIKeyInput, the scanner calls the insertText: protocol method. If it conforms to UITextInput, the scanner calls the setMarkedText(_:selectedRange:) and unmarkText() protocol methods.

To determine whether the data scanner runs on the user’s device, pass captureTextFromCamera(_:) to the canPerformAction(_:withSender:) method.

## See Also

### Related Documentation

Scanning data with the camera

Enable Live Text data scanning of text and codes that appear in the camera’s viewfinder.

