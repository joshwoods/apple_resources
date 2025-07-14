

- UIKit
-  UITextViewDelegate 

Protocol

# UITextViewDelegate

The methods for receiving editing-related messages for text view objects.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UITextViewDelegate : UIScrollViewDelegate
```

## Overview

All of the methods in this protocol are optional. You can use them in situations where you might want to adjust the text a user is editing (such as in the case of a spell-checker program) or to modify the intended insertion point.

## Topics

### Responding to editing notifications

func textViewShouldBeginEditing(UITextView) -> Bool

Asks the delegate whether to begin editing in the specified text view.

func textViewDidBeginEditing(UITextView)

Tells the delegate when editing of the specified text view begins.

func textViewShouldEndEditing(UITextView) -> Bool

Asks the delegate whether to stop editing in the specified text view.

func textViewDidEndEditing(UITextView)

Tells the delegate when editing of the specified text view ends.

### Responding to text changes

func textView(UITextView, shouldChangeTextIn: NSRange, replacementText: String) -> Bool

Asks the delegate whether to replace the specified text in the text view.

func textViewDidChange(UITextView)

Tells the delegate when the user changes the text or attributes in the specified text view.

### Responding to selection changes

func textViewDidChangeSelection(UITextView)

Tells the delegate when the text selection changes in the specified text view.

### Interacting with text data

func textView(UITextView, menuConfigurationFor: UITextItem, defaultMenu: UIMenu) -> UITextItem.MenuConfiguration?

func textView(UITextView, primaryActionFor: UITextItem, defaultAction: UIAction) -> UIAction?

func textView(UITextView, textItemMenuWillDisplayFor: UITextItem, animator: any UIContextMenuInteractionAnimating)

func textView(UITextView, textItemMenuWillEndFor: UITextItem, animator: any UIContextMenuInteractionAnimating)

### Providing a context menu

func textView(UITextView, editMenuForTextIn: NSRange, suggestedActions: [UIMenuElement]) -> UIMenu?

Asks the delegate for the menu to display in the text view, based on the text range and actions the system provides.

### Customizing an edit menu

func textView(UITextView, willDismissEditMenuWith: any UIEditMenuInteractionAnimating)

func textView(UITextView, willPresentEditMenuWith: any UIEditMenuInteractionAnimating)

### Responding to writing tools interactions

func textViewWritingToolsWillBegin(UITextView)

Tells the delegate that an interaction with the writing tools interface is about to begin.

func textViewWritingToolsDidEnd(UITextView)

Tells the delegate that the current writing tools session ended.

func textView(UITextView, writingToolsIgnoredRangesInEnclosingRange: NSRange) -> [NSValue]

Asks the delegate to specify any ranges of text you want the writing tools to ignore.

### Inserting a Smart Reply suggestion

func textView(UITextView, insertInputSuggestion: UIInputSuggestion)

Tells the delegate when the keyboard delivers an input suggestion.

### Deprecated

func textView(UITextView, shouldInteractWith: NSTextAttachment, in: NSRange, interaction: UITextItemInteraction) -> Bool

Asks the delegate whether the specified text view allows the specified type of user interaction with the provided text attachment in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: URL, in: NSRange, interaction: UITextItemInteraction) -> Bool

Asks the delegate whether the specified text view allows the specified type of user interaction with the specified URL in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: NSTextAttachment, in: NSRange) -> Bool

Asks the delegate whether the specified text view allows user interaction with the provided text attachment in the specified range of text.

Deprecated

func textView(UITextView, shouldInteractWith: URL, in: NSRange) -> Bool

Asks the delegate whether the specified text view allows user interaction with the specified URL in the specified range of text.

Deprecated

enum UITextItemInteraction

Constants that indicate the type of interaction the user expects to have with a URL or text attachment.

Deprecated

### Instance Methods

func textView(UITextView, didBeginFormattingWith: UITextFormattingViewController)

func textView(UITextView, didEndFormattingWith: UITextFormattingViewController)

func textView(UITextView, willBeginFormattingWith: UITextFormattingViewController)

func textView(UITextView, willEndFormattingWith: UITextFormattingViewController)

## Relationships

### Inherits From

- NSObjectProtocol
- UIScrollViewDelegate

## See Also

### Text actions and menus

class UITextItem

An object for attaching custom actions and menus to links, text attachments, or other specific text in a text view.

class MenuConfiguration

An object that describes what type of menu and preview to show for a text item.

