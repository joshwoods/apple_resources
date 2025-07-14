

- UIKit
- UISearchTextField
-  tokens 

Instance Property

# tokens

The collection of tokens in the search text field.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var tokens: [UISearchToken] { get set }
```

## Discussion

Use this property to access existing tokens, or to replace all tokens at once. To convert text in the search field into a token, use replaceTextualPortion(of:with:at:).

## See Also

### Adding and removing tokens

func insertToken(UISearchToken, at: Int)

Adds a search token at a specific index.

func removeToken(at: Int)

Removes a particular search token from the search text field.

