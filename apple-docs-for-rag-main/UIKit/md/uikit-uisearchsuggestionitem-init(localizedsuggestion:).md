

- UIKit
- UISearchSuggestionItem
-  init(localizedSuggestion:) 

Initializer

# init(localizedSuggestion:)

Creates a search suggestion with the specified label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(localizedSuggestion suggestion: String)
```

## Parameters 

`suggestion`  

The item’s label, usually the search term.

## See Also

### Creating a search suggestion

init(localizedSuggestion: String, localizedDescription: String?, iconImage: UIImage?)

Creates a search suggestion with the specified text and image attributes.

init(localizedAttributedSuggestion: NSAttributedString, localizedDescription: String?, iconImage: UIImage?)

Creates a search suggestion with the specified attributed label, accessibility description, and image.

init(localizedSuggestion: String, localizedDescription: String?)

Creates a search suggestion with the specified label and accessibility description.

init(localizedAttributedSuggestion: NSAttributedString, localizedDescription: String?)

Creates a search suggestion with the specified attributed label and accessibility description.

init(localizedAttributedSuggestion: NSAttributedString)

Creates a search suggestion with the specified attributed label.

