

- UIKit
-  UITextPasteConfigurationSupporting 

Protocol

# UITextPasteConfigurationSupporting

The interface for text-oriented responder objects to participate in the unified paste and drop system in iOS.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextPasteConfigurationSupporting : UIPasteConfigurationSupporting
```

## Topics

### Setting the text paste delegate

var pasteDelegate: (any UITextPasteDelegate)?

The text paste delegate that handles pasting and dropping of text, using item providers.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIPasteConfigurationSupporting

### Inherited By

- UITextDroppable

### Conforming Types

- UISearchTextField
- UITextField
- UITextView

## See Also

### Pasteboard support

protocol UITextPasteItem

The interface for obtaining information about, and interacting with, a text item for pasting or dropping.

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

protocol UITextPasteDelegate

The interface for handling pasting and dropping of text, using item providers.

