

- UIKit
-  UITextPasteDelegate 

Protocol

# UITextPasteDelegate

The interface for handling pasting and dropping of text, using item providers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextPasteDelegate : NSObjectProtocol
```

## Topics

### Preparing to paste a text paste item

func textPasteConfigurationSupporting(any UITextPasteConfigurationSupporting, transform: any UITextPasteItem)

Tells the delegate to transform the pasted or dropped text item.

### Pasting the text paste item

func textPasteConfigurationSupporting(any UITextPasteConfigurationSupporting, combineItemAttributedStrings: [NSAttributedString], for: UITextRange) -> NSAttributedString

Asks the delegate to combine multiple strings into a single attributed string.

func textPasteConfigurationSupporting(any UITextPasteConfigurationSupporting, performPasteOf: NSAttributedString, to: UITextRange) -> UITextRange

Asks the delegate to explicitly handle the final incorporation of a pasted or dropped string of text into the text view.

### Animating the paste operation

func textPasteConfigurationSupporting(any UITextPasteConfigurationSupporting, shouldAnimatePasteOf: NSAttributedString, to: UITextRange) -> Bool

Asks the delegate if the paste or drop operation should be animated.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Pasteboard support

protocol UITextPasteItem

The interface for obtaining information about, and interacting with, a text item for pasting or dropping.

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

protocol UITextPasteConfigurationSupporting

The interface for text-oriented responder objects to participate in the unified paste and drop system in iOS.

