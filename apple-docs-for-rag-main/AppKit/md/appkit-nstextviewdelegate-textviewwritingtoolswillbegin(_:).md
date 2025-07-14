

- AppKit
- NSTextViewDelegate
-  textViewWritingToolsWillBegin(\_:) 

Instance Method

# textViewWritingToolsWillBegin(\_:)

macOS 15.0+

``` source
@MainActor
optional func textViewWritingToolsWillBegin(_ textView: NSTextView)
```

## Mentioned in 

Customizing Writing Tools behavior for AppKit views

## See Also

### Responding to writing tools interactions

func textViewWritingToolsDidEnd(NSTextView)

func textView(NSTextView, writingToolsIgnoredRangesInEnclosingRange: NSRange) -> [NSValue]

