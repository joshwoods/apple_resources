

- WebKit
- WebHistory
-  orderedItemsLastVisited(onDay:) Deprecated

Instance Method

# orderedItemsLastVisited(onDay:)

Returns web history items that were last visited on the specified date.

macOS 10.3–10.14Deprecated

``` source
func orderedItemsLastVisited(onDay calendarDate: NSCalendarDate!) -> [Any]!
```

## Parameters 

`calendarDate`  

The date on which the web history items were last visited.

## Return Value

An array of web history items that were last visited on the specified date.

## See Also

### Getting Web History Items

var orderedLastVisitedDays: [Any]!

An array of all calendar days represented in the web history.

Deprecated

func item(for: URL!) -> WebHistoryItem!

Returns the web history item that corresponds to the specified web location.

Deprecated

