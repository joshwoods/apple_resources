

- UIKit
- UISearchSuggestionItem
-  init(localizedAttributedSuggestion:) 

Initializer

# init(localizedAttributedSuggestion:)

Creates a search suggestion with the specified attributed label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(localizedAttributedSuggestion suggestion: NSAttributedString)
```

## Parameters 

`suggestion`  

An attributed label for the suggestion, usually the search term the suggestion represents.

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

init(localizedSuggestion: String)

Creates a search suggestion with the specified label.

