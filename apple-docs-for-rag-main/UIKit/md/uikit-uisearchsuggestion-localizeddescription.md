

- UIKit
- UISearchSuggestion
-  localizedDescription 

Instance Property

# localizedDescription

A description of the suggestion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional var localizedDescription: String? { get }
```

## Discussion

The system uses this description for accessibility.

## See Also

### Describing a search suggestion

var localizedSuggestion: String?

A label for the suggestion, usually the search term the suggestion represents.

**Required**

var localizedAttributedSuggestion: NSAttributedString?

An attributed label for the suggestion, usually the search term the suggestion represents.

**Required**

var iconImage: UIImage?

An image for display on the suggestion.

var representedObject: Any?

An object for tracking supplementary information about the search suggestion.

**Required**

