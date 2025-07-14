

- UIKit
- UISearchSuggestionItem
-  localizedAttributedSuggestion 

Instance Property

# localizedAttributedSuggestion

An attributed label for the suggestion, usually the search term the suggestion represents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var localizedAttributedSuggestion: NSAttributedString? { get }
```

## See Also

### Describing a search suggestion

var localizedSuggestion: String?

A label for the suggestion, usually the search term the suggestion represents.

var localizedDescription: String?

A description of the suggestion.

var iconImage: UIImage?

An image for display on the suggestion.

var representedObject: Any?

An object for tracking supplementary information about the search suggestion.

