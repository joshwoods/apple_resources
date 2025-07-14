

- UIKit
- UISearchTextField
-  positionOfToken(at:) 

Instance Method

# positionOfToken(at:)

Converts a token index into a text position.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func positionOfToken(at tokenIndex: Int) -> UITextPosition
```

## Parameters 

`tokenIndex`  

The array index of the token.

## Return Value

The text position of the token.

## Discussion

Use this method to convert a token’s index in the tokens array into the token’s UITextPosition in the overall contents of the text field. Many UITextInput methods for interacting with text take a UITextPosition or UITextRange (constructed from two text positions) as a parameter.

To select a search token, assign a UITextRange that contains the token’s position to the selectedTextRange property.

## See Also

### Customizing token behavior

var tokenBackgroundColor: UIColor!

The background color for all tokens in the search text field.

func tokens(in: UITextRange) -> [UISearchToken]

Returns the search field’s tokens that are within a given range.

