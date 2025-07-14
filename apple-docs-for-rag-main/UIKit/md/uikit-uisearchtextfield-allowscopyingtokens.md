

- UIKit
- UISearchTextField
-  allowsCopyingTokens 

Instance Property

# allowsCopyingTokens

A Boolean that indicates whether the user can copy or drag tokens from the search field.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsCopyingTokens: Bool { get set }
```

## Discussion

The default value for this property is true.

To support copying tokens, allowsCopyingTokens must be true and the search field’s delegate must also implement searchTextField(_:itemProviderForCopying:).

UISearchTextField enables the Copy command when a user selects text, even if the selection also includes tokens and allowsCopyingTokens is false.

## See Also

### Supporting token interactions

var allowsDeletingTokens: Bool

A Boolean that indicates whether the user can remove tokens from the search field.

var delegate: (any UITextFieldDelegate)?

The text field’s delegate.

protocol UISearchTextFieldDelegate

The interface for the delegate of a search field.

protocol UISearchTextFieldPasteItem

A protocol that supports pasting tokens.

