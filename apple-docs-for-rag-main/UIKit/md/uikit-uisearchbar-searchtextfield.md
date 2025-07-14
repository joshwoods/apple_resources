

- UIKit
- UISearchBar
-  searchTextField 

Instance Property

# searchTextField

The text field that the user enters a search query into.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var searchTextField: UISearchTextField { get }
```

## Discussion

For details about interacting with the text field, accessing its content, and using tokens, see UISearchTextField and UISearchToken.

## See Also

### Getting the search text

var placeholder: String?

The string to display when there’s no other text in the text field.

var prompt: String?

A single line of text displayed at the top of the search bar.

var text: String?

The current or starting search text.

