

- AppKit
- NSTextViewDelegate
-  textView(\_:writingToolsIgnoredRangesInEnclosingRange:) 

Instance Method

# textView(\_:writingToolsIgnoredRangesInEnclosingRange:)

macOS 15.0+

``` source
@MainActor
optional func textView(
    _ textView: NSTextView,
    writingToolsIgnoredRangesInEnclosingRange enclosingRange: NSRange
) -> [NSValue]
```

## Mentioned in 

Customizing Writing Tools behavior for AppKit views

## See Also

### Responding to writing tools interactions

func textViewWritingToolsWillBegin(NSTextView)

func textViewWritingToolsDidEnd(NSTextView)

