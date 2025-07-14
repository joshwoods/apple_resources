

- AppKit
- NSSearchField
-  recentsAutosaveName 

Instance Property

# recentsAutosaveName

The name under which the search field automatically archives the list of recent search strings.

macOS

``` source
@MainActor
var recentsAutosaveName: NSSearchField.RecentsAutosaveName? { get set }
```

## Discussion

Used as a key in the standard user defaults to save the recent searches. If you specify `nil` or an empty string for this property, no autosave name is set and searches aren’t autosaved.

## See Also

### Managing Recent Searches

var recentSearches: [String]

The list of recent search strings for the control.

var maximumRecents: Int

The maximum number of search strings that can appear in the search menu.

typealias RecentsAutosaveName

The string that stores the name under which a search field automatically archives a list of recent search strings.

