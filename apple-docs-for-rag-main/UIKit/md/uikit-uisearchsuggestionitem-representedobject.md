

- UIKit
- UISearchSuggestionItem
-  representedObject 

Instance Property

# representedObject

An object for tracking supplementary information about the search suggestion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var representedObject: Any? { get set }
```

## Discussion

Use this property to associate the search suggestion with a corresponding object.

## See Also

### Describing a search suggestion

var localizedSuggestion: String?

A label for the suggestion, usually the search term the suggestion represents.

var localizedAttributedSuggestion: NSAttributedString?

An attributed label for the suggestion, usually the search term the suggestion represents.

var localizedDescription: String?

A description of the suggestion.

var iconImage: UIImage?

An image for display on the suggestion.

