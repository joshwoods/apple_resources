

- UIKit
- UISearchTextField
-  removeToken(at:) 

Instance Method

# removeToken(at:)

Removes a particular search token from the search text field.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func removeToken(at tokenIndex: Int)
```

## Parameters 

`tokenIndex`  

Within the tokens array, the index of the token you want to remove.

## See Also

### Adding and removing tokens

var tokens: [UISearchToken]

The collection of tokens in the search text field.

func insertToken(UISearchToken, at: Int)

Adds a search token at a specific index.

