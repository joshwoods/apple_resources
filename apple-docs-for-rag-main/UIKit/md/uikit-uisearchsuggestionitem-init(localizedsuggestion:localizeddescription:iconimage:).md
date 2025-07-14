

- UIKit
- UISearchSuggestionItem
-  init(localizedSuggestion:localizedDescription:iconImage:) 

Initializer

# init(localizedSuggestion:localizedDescription:iconImage:)

Creates a search suggestion with the specified text and image attributes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(
    localizedSuggestion suggestion: String,
    localizedDescription description: String?,
    iconImage: UIImage?
)
```

## Parameters 

`suggestion`  

A label for the suggestion, usually the search term the suggestion represents.

`description`  

A description of the suggestion. The system uses this description for accessibility.

`iconImage`  

An image for display on the suggestion.

## See Also

### Creating a search suggestion

init(localizedAttributedSuggestion: NSAttributedString, localizedDescription: String?, iconImage: UIImage?)

Creates a search suggestion with the specified attributed label, accessibility description, and image.

init(localizedSuggestion: String, localizedDescription: String?)

Creates a search suggestion with the specified label and accessibility description.

init(localizedAttributedSuggestion: NSAttributedString, localizedDescription: String?)

Creates a search suggestion with the specified attributed label and accessibility description.

init(localizedSuggestion: String)

Creates a search suggestion with the specified label.

init(localizedAttributedSuggestion: NSAttributedString)

Creates a search suggestion with the specified attributed label.

