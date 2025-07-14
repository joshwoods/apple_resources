

- UIKit
- UISearchTextField
-  insertToken(\_:at:) 

Instance Method

# insertToken(\_:at:)

Adds a search token at a specific index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func insertToken(
    _ token: UISearchToken,
    at tokenIndex: Int
)
```

## Parameters 

`token`  

The search token to be inserted.

`tokenIndex`  

Within the tokens array, the index at which to insert the token.

## Discussion

If you’re converting part of the search field’s text into a token, use replaceTextualPortion(of:with:at:).

## See Also

### Adding and removing tokens

var tokens: [UISearchToken]

The collection of tokens in the search text field.

func removeToken(at: Int)

Removes a particular search token from the search text field.

