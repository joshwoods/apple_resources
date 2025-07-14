

- WebKit
-  WebHistoryItem Deprecated

Class

# WebHistoryItem

WebHistoryItem objects encapsulate information about visiting a page so that users can return to that page. WebHistory and WebBackForwardList objects manage lists of WebHistoryItem objects. WebHistoryItem objects are created and added to these lists automatically when loading pages, so you do not need to create WebHistoryItem objects directly.

macOS 10.3–10.14Deprecated

``` source
class WebHistoryItem
```

## Topics

### Initializing WebHistoryItem objects

init!(urlString: String!, title: String!, lastVisitedTimeInterval: TimeInterval)

Initializes the receiver with a URL,`URLString`, a title specified by `title` and the last time this item was visited specified by `time` title, and time last visited.

### Getting URL information

var urlString: String!

The string representation of the URL for the receiver’s page.

var originalURLString: String!

The string representation of the original URL for the receiver’s page.

### Getting and setting page titles

var title: String!

The receiver’s original page title.

var alternateTitle: String!

An alternate title that may be used in place of the receiver’s page title.

### Getting other attributes

var icon: NSImage!

The icon for the receiver’s page, or `nil` if none exists.

var lastVisitedTimeInterval: TimeInterval

The last time and date the receiver’s page was visited.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Accessing Previous Webpages (Legacy)

class WebBackForwardList

A `WebBackForwardList` object maintains a list of visited pages used to go back and forward to the most recent page. A `WebBackForwardList` object maintains only the list data—it does not perform actual page loads (in other words, it does not make any client requests). If you need to perform a page load, see the load(_:) method in WebFrame to find out how to do this.

Deprecated

class WebHistory

`WebHistory` objects are used to maintain the pages visited by users. Visited pages are represented by WebHistoryItem objects. You add and remove history items using the addItems(_:) and removeItems(_:) methods. These methods post appropriate notifications when items are added or removed so you can update the display. `WebHistory` organizes the `WebHistoryItem` objects by the day they were visited, ordered from most recent to oldest. You can request all the days that contain history items using the orderedLastVisitedDays method or request the items visited on a particular day using the orderedItemsLastVisited(onDay:) method. `WebHistory` objects can be loaded and saved by specifying a file URL (see load(from:)).

Deprecated

