

- UIKit
- UITextViewDelegate
-  textViewWritingToolsWillBegin(\_:) 

Instance Method

# textViewWritingToolsWillBegin(\_:)

Tells the delegate that an interaction with the writing tools interface is about to begin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
@MainActor
optional func textViewWritingToolsWillBegin(_ textView: UITextView)
```

## Parameters 

`textView`  

The text view that is about to begin a writing tools session.

## Mentioned in 

Customizing Writing Tools behavior for UIKit views

## Discussion

Use this method to take any necessary steps to prepare your app for writing tools interactions. During the course of a writing tools session, the writing tools UI suggests changes to the text view’s text. It also allows the person to toggle between the original and replacement text before choosing one. To avoid issues while these changes occur, save any current data to disk and and disable features that might modify your view’s text storage while the session is active. For example, disable iCloud synchronization until the session ends. Reenable those features when the session ends.

The text view calls this method when the person requests the writing tools interface, but before the interface makes any changes to your content. Because the session isn’t active yet, the isWritingToolsActive property of the text view is false while this method executes. The value of that property resolves to true only after the method returns.

## See Also

### Responding to writing tools interactions

func textViewWritingToolsDidEnd(UITextView)

Tells the delegate that the current writing tools session ended.

func textView(UITextView, writingToolsIgnoredRangesInEnclosingRange: NSRange) -> [NSValue]

Asks the delegate to specify any ranges of text you want the writing tools to ignore.

