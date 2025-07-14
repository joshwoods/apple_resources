

- AppKit
- NSTextFieldDelegate
-  textField(\_:textView:candidates:forSelectedRange:) 

Instance Method

# textField(\_:textView:candidates:forSelectedRange:)

macOS 10.12.2+

``` source
@MainActor
optional func textField(
    _ textField: NSTextField,
    textView: NSTextView,
    candidates: [NSTextCheckingResult],
    forSelectedRange selectedRange: NSRange
) -> [NSTextCheckingResult]
```

## See Also

### Controlling Editing Behavior

func textField(NSTextField, textView: NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

func textField(NSTextField, textView: NSTextView, shouldSelectCandidateAt: Int) -> Bool

