

- AppKit
- NSTextFieldDelegate
-  textField(\_:textView:candidatesForSelectedRange:) 

Instance Method

# textField(\_:textView:candidatesForSelectedRange:)

macOS 10.12.2+

``` source
@MainActor
optional func textField(
    _ textField: NSTextField,
    textView: NSTextView,
    candidatesForSelectedRange selectedRange: NSRange
) -> [Any]?
```

## See Also

### Controlling Editing Behavior

func textField(NSTextField, textView: NSTextView, candidates: [NSTextCheckingResult], forSelectedRange: NSRange) -> [NSTextCheckingResult]

func textField(NSTextField, textView: NSTextView, shouldSelectCandidateAt: Int) -> Bool

