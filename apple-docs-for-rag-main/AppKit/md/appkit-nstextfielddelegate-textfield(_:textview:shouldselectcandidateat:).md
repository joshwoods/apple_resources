

- AppKit
- NSTextFieldDelegate
-  textField(\_:textView:shouldSelectCandidateAt:) 

Instance Method

# textField(\_:textView:shouldSelectCandidateAt:)

macOS 10.12.2+

``` source
@MainActor
optional func textField(
    _ textField: NSTextField,
    textView: NSTextView,
    shouldSelectCandidateAt index: Int
) -> Bool
```

## See Also

### Controlling Editing Behavior

func textField(NSTextField, textView: NSTextView, candidates: [NSTextCheckingResult], forSelectedRange: NSRange) -> [NSTextCheckingResult]

func textField(NSTextField, textView: NSTextView, candidatesForSelectedRange: NSRange) -> [Any]?

