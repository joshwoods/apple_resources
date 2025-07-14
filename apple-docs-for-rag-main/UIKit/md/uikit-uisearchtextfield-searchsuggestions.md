

- UIKit
- UISearchTextField
-  searchSuggestions 

Instance Property

# searchSuggestions

A list of suggestions to offer as shortcuts below the search field.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var searchSuggestions: [any UISearchSuggestion]? { get set }
```

## Mentioned in 

Building a desktop-class iPad app

## Discussion

Provide search suggestions to help people complete their query quickly. Update the suggestions as a person types by registering for the textDidChangeNotification notification and implementing textFieldDidEndEditing(_:reason:).

The suggestions appear in a menu under the search field. When you assign new suggestions to this property, the suggestions onscreen refresh automatically. When a person chooses a suggestion, the system sets this property to `nil` and dismisses the search suggestions menu. Implement searchTextField(_:didSelect:) in your delegate to execute any necessary updates when a person chooses a suggestion.

If the search suggestions menu dismisses for other reasons, such as a person tapping outside the search bar, searchSuggestions doesn’t reset to `nil` immediately. The system sets searchSuggestions to `nil` only when a person interacts with search directly — for example, by typing in the search field, canceling search, or changing the search scope using the search bar’s scope bar. To dismiss the menu manually, set this property to `nil` or `[]`.

Important

UIKit allows setting this property directly on an instance of UISearchTextField only when the search field isn’t associated with a UISearchController. If the search field is associated with a search controller, the system raises an invalidArgumentException to use the searchSuggestions property on UISearchController instead.

