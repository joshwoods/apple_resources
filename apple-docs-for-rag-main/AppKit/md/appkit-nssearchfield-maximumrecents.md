

- AppKit
- NSSearchField
-  maximumRecents 

Instance Property

# maximumRecents

The maximum number of search strings that can appear in the search menu.

macOS 10.10+

``` source
@MainActor
var maximumRecents: Int { get set }
```

## Discussion

The value of this property must be between 0 and 254. Specifying a negative value for the property sets it to the default value, which is 10. Specifying a value greater than 254 sets the property to 254.

When the maximum number of search strings is exceeded, the oldest search string on the menu is dropped.

## See Also

### Managing Recent Searches

var recentSearches: [String]

The list of recent search strings for the control.

var recentsAutosaveName: NSSearchField.RecentsAutosaveName?

The name under which the search field automatically archives the list of recent search strings.

typealias RecentsAutosaveName

The string that stores the name under which a search field automatically archives a list of recent search strings.

