

- WebKit
- WebHistory
-  item(for:) Deprecated

Instance Method

# item(for:)

Returns the web history item that corresponds to the specified web location.

macOS 10.3–10.14Deprecated

``` source
func item(for URL: URL!) -> WebHistoryItem!
```

## Parameters 

`URL`  

The location, as a URL, of the webpage that was visited.

## Return Value

The web history item that represents visits to the specified URL, or `nil` if none was found.

## See Also

### Getting Web History Items

func orderedItemsLastVisited(onDay: NSCalendarDate!) -> [Any]!

Returns web history items that were last visited on the specified date.

Deprecated

var orderedLastVisitedDays: [Any]!

An array of all calendar days represented in the web history.

Deprecated

