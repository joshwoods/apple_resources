

- UIKit
- UISearchTextField
-  allowsDeletingTokens 

Instance Property

# allowsDeletingTokens

A Boolean that indicates whether the user can remove tokens from the search field.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsDeletingTokens: Bool { get set }
```

## Discussion

The default value for this property is true.

You can always remove tokens programmatically. When this value is true, the user can also delete tokens and your app needs to handle tokens being re-added to the field with Undo.

## See Also

### Supporting token interactions

var allowsCopyingTokens: Bool

A Boolean that indicates whether the user can copy or drag tokens from the search field.

var delegate: (any UITextFieldDelegate)?

The text field’s delegate.

protocol UISearchTextFieldDelegate

The interface for the delegate of a search field.

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

