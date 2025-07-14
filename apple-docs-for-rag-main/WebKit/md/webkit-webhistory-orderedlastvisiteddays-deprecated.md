

- WebKit
- WebHistory
-  orderedLastVisitedDays Deprecated

Instance Property

# orderedLastVisitedDays

An array of all calendar days represented in the web history.

macOS 10.3–10.14Deprecated

``` source
var orderedLastVisitedDays: [Any]! { get }
```

## See Also

### Getting Web History Items

func orderedItemsLastVisited(onDay: NSCalendarDate!) -> [Any]!

Returns web history items that were last visited on the specified date.

Deprecated

func item(for: URL!) -> WebHistoryItem!

Returns the web history item that corresponds to the specified web location.

Deprecated

