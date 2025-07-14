

- AppKit
- NSSearchFieldCell
-  maximumRecents 

Instance Property

# maximumRecents

The maximum number of search strings that can appear in the search menu.

macOS

``` source
@MainActor
var maximumRecents: Int { get set }
```

## Discussion

The value of this property must be between `0` and `254`. Specifying a negative value for the property sets it to the default value, which is `10`. Specifying a value greater than `254` sets the property to `254`.

When the maximum number of search strings is exceeded, the oldest search string on the menu is dropped.

## See Also

### Managing recent search strings

var recentSearches: [String]!

An array of the recent search strings to display in the pop-up icon menu of the search field.

var recentsAutosaveName: NSSearchField.RecentsAutosaveName?

The autosave name under which the search field automatically saves the list of recent search strings.

