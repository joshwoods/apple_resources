

- UIKit
- UISearchTextField
-  tokens(in:) 

Instance Method

# tokens(in:)

Returns the search field’s tokens that are within a given range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func tokens(in textRange: UITextRange) -> [UISearchToken]
```

## Parameters 

`textRange`  

The range specifying a subset of the tokens.

## Return Value

The tokens contained within the provided range.

## Discussion

Use this method to find out which tokens are included in the user’s current selection. You can provide a range that spans a mixture of tokens and text.

## See Also

### Customizing token behavior

var tokenBackgroundColor: UIColor!

The background color for all tokens in the search text field.

func positionOfToken(at: Int) -> UITextPosition

Converts a token index into a text position.

