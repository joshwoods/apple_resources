

- UIKit
- UISearchBar
-  prompt 

Instance Property

# prompt

A single line of text displayed at the top of the search bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var prompt: String? { get set }
```

## Discussion

The default value is `nil`.

## See Also

### Getting the search text

var placeholder: String?

The string to display when there’s no other text in the text field.

var text: String?

The current or starting search text.

var searchTextField: UISearchTextField

The text field that the user enters a search query into.

