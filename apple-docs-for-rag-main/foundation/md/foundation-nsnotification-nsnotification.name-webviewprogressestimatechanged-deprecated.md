

- Foundation
- NSNotification
- NSNotification.Name
-  WebViewProgressEstimateChanged Deprecated

Type Property

# WebViewProgressEstimateChanged

Posted by a WebView object when the estimated progress value of a load changes.

macOS 10.3–10.14Deprecated

``` source
static let WebViewProgressEstimateChanged: NSNotification.Name
```

## Discussion

This notification may be posted zero or more times after a WebViewProgressStarted notification is posted. The notification object is the WebView for which the progress value has changed. This notification does not contain a `userInfo` dictionary.

## See Also

### WebKit

static let WebHistoryAllItemsRemoved: NSNotification.Name

Posted when all history items have been removed from the web history.

Deprecated

static let WebHistoryItemChanged: NSNotification.Name

Posted by a WebHistoryItem object when the value of the history item’s title, alternate title, URL strings, or last visited interval changes.

Deprecated

static let WebHistoryItemsAdded: NSNotification.Name

Posted when history items have been added to a web history.

Deprecated

static let WebHistoryItemsRemoved: NSNotification.Name

Posted when items have been removed from the web history.

Deprecated

static let WebHistoryLoaded: NSNotification.Name

Posted when web history items have been loaded from a URL.

Deprecated

static let WebHistorySaved: NSNotification.Name

Posted when web history items have been saved to a URL.

Deprecated

static let WebPreferencesChanged: NSNotification.Name

Posted when the web preference settings are changed.

Deprecated

static let WebViewDidBeginEditing: NSNotification.Name

Posted when a web view begins any operation that changes its contents in response to user editing.

Deprecated

static let WebViewDidChange: NSNotification.Name

Posted when a web view performs any operation that changes its contents in response to user editing.

Deprecated

static let WebViewDidChangeSelection: NSNotification.Name

Posted when a web view changes its typing selection.

Deprecated

static let WebViewDidChangeTypingStyle: NSNotification.Name

Posted when a web view changes its typing style.

Deprecated

static let WebViewDidEndEditing: NSNotification.Name

Posted when a web view ends any operation that changes its contents in response to user editing.

Deprecated

static let WebViewProgressFinished: NSNotification.Name

Posted by a WebView object when the load has finished.

Deprecated

static let WebViewProgressStarted: NSNotification.Name

Posted by a WebView object when a load begins, including a load that is initiated in a subframe.

Deprecated

