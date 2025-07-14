

- WebKit
-  WebHistory Deprecated

Class

# WebHistory

`WebHistory` objects are used to maintain the pages visited by users. Visited pages are represented by WebHistoryItem objects. You add and remove history items using the addItems(_:) and removeItems(_:) methods. These methods post appropriate notifications when items are added or removed so you can update the display. `WebHistory` organizes the `WebHistoryItem` objects by the day they were visited, ordered from most recent to oldest. You can request all the days that contain history items using the orderedLastVisitedDays method or request the items visited on a particular day using the orderedItemsLastVisited(onDay:) method. `WebHistory` objects can be loaded and saved by specifying a file URL (see load(from:)).

macOS 10.3–10.14Deprecated

``` source
class WebHistory
```

## Topics

### Accessing Shared History Objects

class func optionalShared() -> WebHistory!

Returns a shared web history object, if one exists.

class func setOptionalShared(WebHistory!)

Sets the web history object to share.

### Adding and Removing History Items

func addItems([Any]!)

Inserts or updates the specified items in the web history.

func removeItems([Any]!)

Removes the specified items from the web history.

func removeAllItems()

Removes all items from the web history.

### Getting Web History Items

func orderedItemsLastVisited(onDay: NSCalendarDate!) -> [Any]!

Returns web history items that were last visited on the specified date.

var orderedLastVisitedDays: [Any]!

An array of all calendar days represented in the web history.

func item(for: URL!) -> WebHistoryItem!

Returns the web history item that corresponds to the specified web location.

### Loading and Saving History Information

func load(from: URL!) throws

Loads the contents of the specified web history file.

func save(to: URL!) throws

Saves the web history to the specified file.

### Getting and Setting Attributes

var historyAgeInDaysLimit: Int32

The maximum age of web history items that can be retrieved.

var historyItemLimit: Int32

The maximum number of web history items that can be stored.

### Constants

Web History Dictionary Keys

The key for accessing the web history items stored in a notification’s user information dictionary.

### Notifications

static let WebHistoryAllItemsRemoved: NSNotification.Name

Posted when all history items have been removed from the web history.

static let WebHistoryItemChanged: NSNotification.Name

Posted by a WebHistoryItem object when the value of the history item’s title, alternate title, URL strings, or last visited interval changes.

static let WebHistoryItemsAdded: NSNotification.Name

Posted when history items have been added to a web history.

static let WebHistoryItemsRemoved: NSNotification.Name

Posted when items have been removed from the web history.

static let WebHistoryLoaded: NSNotification.Name

Posted when web history items have been loaded from a URL.

static let WebHistorySaved: NSNotification.Name

Posted when web history items have been saved to a URL.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accessing Previous Webpages (Legacy)

class WebBackForwardList

A `WebBackForwardList` object maintains a list of visited pages used to go back and forward to the most recent page. A `WebBackForwardList` object maintains only the list data—it does not perform actual page loads (in other words, it does not make any client requests). If you need to perform a page load, see the load(_:) method in WebFrame to find out how to do this.

Deprecated

class WebHistoryItem

WebHistoryItem objects encapsulate information about visiting a page so that users can return to that page. WebHistory and WebBackForwardList objects manage lists of WebHistoryItem objects. WebHistoryItem objects are created and added to these lists automatically when loading pages, so you do not need to create WebHistoryItem objects directly.

Deprecated

