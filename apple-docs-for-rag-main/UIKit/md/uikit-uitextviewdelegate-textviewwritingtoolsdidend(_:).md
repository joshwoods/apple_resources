

- UIKit
- UITextViewDelegate
-  textViewWritingToolsDidEnd(\_:) 

Instance Method

# textViewWritingToolsDidEnd(\_:)

Tells the delegate that the current writing tools session ended.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
@MainActor
optional func textViewWritingToolsDidEnd(_ textView: UITextView)
```

## Parameters 

`textView`  

The text view that ended a writing tools session.

## Mentioned in 

Customizing Writing Tools behavior for UIKit views

## Discussion

Use this method to undo any actions you took at the start of a writing tools session to modify your app’s behavior. The text view calls this method after the writing session finishes. At this point, the text view contains the final text the person chose.

## See Also

### Responding to writing tools interactions

func textViewWritingToolsWillBegin(UITextView)

Tells the delegate that an interaction with the writing tools interface is about to begin.

func textView(UITextView, writingToolsIgnoredRangesInEnclosingRange: NSRange) -> [NSValue]

Asks the delegate to specify any ranges of text you want the writing tools to ignore.

