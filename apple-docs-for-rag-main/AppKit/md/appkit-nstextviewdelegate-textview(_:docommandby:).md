

- AppKit
- NSTextViewDelegate
-  textView(\_:doCommandBy:) 

Instance Method

# textView(\_:doCommandBy:)

Sent to allow the delegate to perform the command for the text view.

macOS 10.0+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    doCommandBy commandSelector: Selector
) -> Bool
```

## Parameters 

`textView`  

The text view sending the message. This is the first text view in a series shared by a layout manager.

`commandSelector`  

The selector.

## Return Value

true indicates that the delegate handled the command and the text view will not attempt to perform it; false indicates that the delegate did not handle the command the text view will attempt to perform it.

## Discussion

This method is invoked by `NSTextView`’s `doCommand(by:)` method.

