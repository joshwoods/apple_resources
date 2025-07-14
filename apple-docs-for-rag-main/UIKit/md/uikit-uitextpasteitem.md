

- UIKit
-  UITextPasteItem 

Protocol

# UITextPasteItem

The interface for obtaining information about, and interacting with, a text item for pasting or dropping.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextPasteItem : NSObjectProtocol
```

## Topics

### Accessing the text paste item’s data

var itemProvider: NSItemProvider

The item provider for the item being pasted or dropped.

**Required**

var localObject: Any?

The custom local object that the copy or drag source optionally attached to the drag item.

**Required**

### Getting the default attributes for a string

var defaultAttributes: [NSAttributedString.Key : Any]

The dictionary of default attributes that the system applies, during pasting or dropping, to plaintext strings from an item provider.

**Required**

### Setting a text paste item’s result value

func setResult(string: String)

Sets a text paste item’s textual value to a specified plaintext string from the item provider.

**Required**

func setResult(attributedString: NSAttributedString)

Sets a text paste item’s textual value to a specified attributed string from the item provider.

**Required**

func setResult(attachment: NSTextAttachment)

Sets a text paste item’s attachment value to a specified value.

**Required**

func setDefaultResult()

Sets the text paste item’s value to the default value based on the item provider’s data.

**Required**

func setNoResult()

Sets the text paste item’s textual value to not include data from the item provider.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UISearchTextFieldPasteItem

## See Also

### Pasteboard support

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

protocol UITextPasteDelegate

The interface for handling pasting and dropping of text, using item providers.

protocol UITextPasteConfigurationSupporting

The interface for text-oriented responder objects to participate in the unified paste and drop system in iOS.

