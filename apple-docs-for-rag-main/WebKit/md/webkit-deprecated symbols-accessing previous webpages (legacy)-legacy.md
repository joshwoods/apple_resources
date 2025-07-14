

- WebKit
- Deprecated Symbols
-  Accessing Previous Webpages (Legacy) 

API Collection

# Accessing Previous Webpages (Legacy)

## Topics

### Accessing Previous Webpages (Legacy)

class WebBackForwardList

A `WebBackForwardList` object maintains a list of visited pages used to go back and forward to the most recent page. A `WebBackForwardList` object maintains only the list data—it does not perform actual page loads (in other words, it does not make any client requests). If you need to perform a page load, see the load(_:) method in WebFrame to find out how to do this.

Deprecated

class WebHistory

`WebHistory` objects are used to maintain the pages visited by users. Visited pages are represented by WebHistoryItem objects. You add and remove history items using the addItems(_:) and removeItems(_:) methods. These methods post appropriate notifications when items are added or removed so you can update the display. `WebHistory` organizes the `WebHistoryItem` objects by the day they were visited, ordered from most recent to oldest. You can request all the days that contain history items using the orderedLastVisitedDays method or request the items visited on a particular day using the orderedItemsLastVisited(onDay:) method. `WebHistory` objects can be loaded and saved by specifying a file URL (see load(from:)).

Deprecated

class WebHistoryItem

WebHistoryItem objects encapsulate information about visiting a page so that users can return to that page. WebHistory and WebBackForwardList objects manage lists of WebHistoryItem objects. WebHistoryItem objects are created and added to these lists automatically when loading pages, so you do not need to create WebHistoryItem objects directly.

Deprecated

## See Also

### WebKit Legacy APIs

Document Object Models API (Legacy)

Setting Up a Web View (Legacy)

Archiving Webpages (Legacy)

Loading Resources (Legacy)

Working with Frames (legacy)

Downloading Information (Legacy)

Opening a File (Legacy)

Setting Policies (Legacy)

Implementing Plugins (Legacy)

Incorporating Scripts (Legacy)

Working With Document Web Views (Legacy)

