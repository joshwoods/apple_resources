

- UIKit
-  UISearchTextFieldDelegate 

Protocol

# UISearchTextFieldDelegate

The interface for the delegate of a search field.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UISearchTextFieldDelegate : UITextFieldDelegate
```

## Overview

A search field asks its delegate for an NSItemProvider when the user starts to copy or move a token. To support these interactions, set the search field’s delegate to an instance of UISearchTextFieldDelegate that implements searchTextField(_:itemProviderForCopying:) and set the search field’s allowsCopyingTokens property to true.

The search field’s pasteDelegate handles pasting and dropping tokens as well as text.

## Topics

### Providing information to copy and drag

func searchTextField(UISearchTextField, itemProviderForCopying: UISearchToken) -> NSItemProvider

Asks the delegate for an object that can provide a token when the copied token is pasted.

### Responding to search suggestion selections

func searchTextField(UISearchTextField, didSelect: any UISearchSuggestion)

Tells the delegate when a person selects a search suggestion in the search text field.

## Relationships

### Inherits From

- NSObjectProtocol
- UITextFieldDelegate

## See Also

### Search field

class UISearchTextField

A view for displaying and editing text and search tokens.

class UISearchToken

Search criteria in a search text field, represented by text and an optional icon.

