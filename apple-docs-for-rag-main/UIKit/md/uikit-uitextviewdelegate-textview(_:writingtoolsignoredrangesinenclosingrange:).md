

- UIKit
- UITextViewDelegate
-  textView(\_:writingToolsIgnoredRangesInEnclosingRange:) 

Instance Method

# textView(\_:writingToolsIgnoredRangesInEnclosingRange:)

Asks the delegate to specify any ranges of text you want the writing tools to ignore.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    writingToolsIgnoredRangesInEnclosingRange enclosingRange: NSRange
) -> [NSValue]
```

## Parameters 

`textView`  

The text view with the active writing tools session.

`enclosingRange`  

The text range that the writing tools are examining. When computing the text ranges to ignore, skip any text that falls outside of this boundary.

## Return Value

One or more ranges of text you want the writing tools to ignore. Return an empty array to allow the modification of all the proposed text.

## Mentioned in 

Customizing Writing Tools behavior for UIKit views

## Discussion

Use this method to prevent the writing tools session from modifying portions of the current text. For example, you might prevent the writing tools session from modifying code or read-only text. The text view provides you with the overall range of text to consider, and you return one or more subranges you want the writing tools to ignore.

## See Also

### Responding to writing tools interactions

func textViewWritingToolsWillBegin(UITextView)

Tells the delegate that an interaction with the writing tools interface is about to begin.

func textViewWritingToolsDidEnd(UITextView)

Tells the delegate that the current writing tools session ended.

