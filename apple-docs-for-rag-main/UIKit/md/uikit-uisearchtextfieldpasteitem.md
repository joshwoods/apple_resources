

- UIKit
-  UISearchTextFieldPasteItem 

Protocol

# UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UISearchTextFieldPasteItem : UITextPasteItem
```

## Overview

When implementing textPasteConfigurationSupporting(_:transform:), your UITextPasteDelegate can decide whether to paste the item as text or as a token. If the UITextPasteItem it receives is a UISearchTextFieldPasteItem, you can call setSearchTokenResult(_:) to prepare a token for pasting instead of text.

## Topics

### Providing a token

func setSearchTokenResult(UISearchToken)

Sets a paste item’s search token from an item provider.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UITextPasteItem

## See Also

### Pasteboard support

protocol UITextPasteItem

The interface for obtaining information about, and interacting with, a text item for pasting or dropping.

protocol UITextPasteDelegate

The interface for handling pasting and dropping of text, using item providers.

protocol UITextPasteConfigurationSupporting

The interface for text-oriented responder objects to participate in the unified paste and drop system in iOS.

