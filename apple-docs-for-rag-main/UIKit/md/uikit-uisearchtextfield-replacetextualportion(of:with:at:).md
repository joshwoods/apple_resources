

- UIKit
- UISearchTextField
-  replaceTextualPortion(of:with:at:) 

Instance Method

# replaceTextualPortion(of:with:at:)

Converts text in a search field into a search token.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func replaceTextualPortion(
    of textRange: UITextRange,
    with token: UISearchToken,
    at tokenIndex: Int
)
```

## Parameters 

`textRange`  

The text to remove.

`token`  

The token to add.

`tokenIndex`  

The location for the added token.

## Discussion

This method removes any text in the specified range, inserts the provided token at the specified index, and selects the newly inserted token. Prefer using this convenience method over performing each step with other methods. When your app calls replaceTextualPortion(of:with:at:), UIKit commits any marked text before modifying the text, and creates a single undo group.

This method doesn’t remove any tokens in the `textRange`, so you don’t have to manually trim the selectedTextRange before you use it in this method.

## See Also

### Converting text into tokens

var textualRange: UITextRange

The range of the field’s text content.

