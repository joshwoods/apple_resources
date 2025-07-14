

- AppKit
- NSSearchField
-  recentSearches 

Instance Property

# recentSearches

The list of recent search strings for the control.

macOS

``` source
@MainActor
var recentSearches: [String] { get set }
```

## Discussion

An array of `NSString` objects, each of which contains a search string either displayed in the search menu or from a recent autosave archive. If there have been no recent searches and no prior searches saved under an autosave name, this array may be empty.

## See Also

### Managing Recent Searches

var maximumRecents: Int

The maximum number of search strings that can appear in the search menu.

var recentsAutosaveName: NSSearchField.RecentsAutosaveName?

The name under which the search field automatically archives the list of recent search strings.

typealias RecentsAutosaveName

The string that stores the name under which a search field automatically archives a list of recent search strings.

