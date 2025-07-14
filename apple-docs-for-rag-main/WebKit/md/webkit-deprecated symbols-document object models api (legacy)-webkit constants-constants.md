

- WebKit
- Deprecated Symbols
- Document Object Models API (Legacy)
-  WebKit Constants 

API Collection

# WebKit Constants

WebKit constants affecting multiple classes.

## Topics

### WKPreview Constants

let WKPreviewActionItemIdentifierAddToReadingList: String

Adds the item to the Reading List.

Deprecated

let WKPreviewActionItemIdentifierCopy: String

Copies the item to the clipboard.

Deprecated

let WKPreviewActionItemIdentifierOpen: String

Opens the item.

Deprecated

let WKPreviewActionItemIdentifierShare: String

Displays the Share panel options available for the item.

Deprecated

### WKWebsiteDataType Constants

let WKWebsiteDataTypeCookies: String

Cookies.

let WKWebsiteDataTypeDiskCache: String

On-disk caches.

let WKWebsiteDataTypeIndexedDBDatabases: String

IndexedDB databases.

let WKWebsiteDataTypeLocalStorage: String

HTML local storage.

let WKWebsiteDataTypeMemoryCache: String

In-memory caches.

let WKWebsiteDataTypeOfflineWebApplicationCache: String

HTML offline web app caches.

let WKWebsiteDataTypeSessionStorage: String

HTML session storage.

let WKWebsiteDataTypeWebSQLDatabases: String

WebSQL databases.

### DOM Constants

let DOMEventException: StringDeprecated

let DOMException: StringDeprecated

let DOMRangeException: StringDeprecated

let DOMXPathException: StringDeprecated

var DOM_BAD_BOUNDARYPOINTS_ERR: DOMRangeExceptionCode

var DOM_DOMSTRING_SIZE_ERR: DOMExceptionCode

var DOM_HIERARCHY_REQUEST_ERR: DOMExceptionCode

var DOM_INDEX_SIZE_ERR: DOMExceptionCode

var DOM_INUSE_ATTRIBUTE_ERR: DOMExceptionCode

var DOM_INVALID_ACCESS_ERR: DOMExceptionCode

var DOM_INVALID_CHARACTER_ERR: DOMExceptionCode

var DOM_INVALID_EXPRESSION_ERR: DOMXPathExceptionCode

var DOM_INVALID_MODIFICATION_ERR: DOMExceptionCode

var DOM_INVALID_NODE_TYPE_ERR: DOMRangeExceptionCode

var DOM_INVALID_STATE_ERR: DOMExceptionCode

var DOM_NAMESPACE_ERR: DOMExceptionCode

var DOM_NOT_FOUND_ERR: DOMExceptionCode

var DOM_NOT_SUPPORTED_ERR: DOMExceptionCode

var DOM_NO_DATA_ALLOWED_ERR: DOMExceptionCode

var DOM_NO_MODIFICATION_ALLOWED_ERR: DOMExceptionCode

var DOM_SYNTAX_ERR: DOMExceptionCode

var DOM_TYPE_ERR: DOMXPathExceptionCode

var DOM_UNSPECIFIED_EVENT_TYPE_ERR: DOMEventExceptionCode

var DOM_WRONG_DOCUMENT_ERR: DOMExceptionCode

### WebKit Constants (Legacy)

let WebActionButtonKey: String

An NSNumber object where `0` indicates the left button, `1` indicates the middle button, and `2` indicates the right button.

Deprecated

let WebActionElementKey: String

A dictionary containing element information. See WebView for a description of the key-value pairs in this dictionary.

Deprecated

let WebActionModifierFlagsKey: String

An unsigned number that indicates the modifier flag.

Deprecated

let WebActionNavigationTypeKey: String

The navigation type of the action. Can be any of the values defined in WebNavigationType below.

Deprecated

let WebActionOriginalURLKey: String

The URL that initiated the action.

Deprecated

let WebArchivePboardType: String

The pasteboard type constant used when adding or accessing a WebArchive on the pasteboard.

Deprecated

let WebElementDOMNodeKey: String

The DOMNode for this element.

Deprecated

let WebElementFrameKey: String

The WebFrame object associated with this element.

Deprecated

let WebElementImageAltStringKey: String

An NSString of the ALT attribute of an image element.

Deprecated

let WebElementImageKey: String

An NSImage representing an image element.

Deprecated

let WebElementImageRectKey: String

An NSValue containing an NSRect, the size of an image element.

Deprecated

let WebElementImageURLKey: String

An NSURL containing the location of an image element.

Deprecated

let WebElementIsSelectedKey: String

An NSNumber used as a BOOL value to indicate whether a text element is selected or not. Zero value indicates false, true otherwise.

Deprecated

let WebElementLinkLabelKey: String

An NSString containing the text within an anchor.

Deprecated

let WebElementLinkTargetFrameKey: String

The WebFrame object associated with the target of the anchor.

Deprecated

let WebElementLinkTitleKey: String

An NSString containing the title of an anchor.

Deprecated

let WebElementLinkURLKey: String

An NSURL containing the location of a link if the element is within an anchor.

Deprecated

static let WebHistoryAllItemsRemoved: NSNotification.Name

Posted when all history items have been removed from the web history.

Deprecated

static let WebHistoryItemChanged: NSNotification.Name

Posted by a WebHistoryItem object when the value of the history item’s title, alternate title, URL strings, or last visited interval changes.

Deprecated

static let WebHistoryItemsAdded: NSNotification.Name

Posted when history items have been added to a web history.

Deprecated

let WebHistoryItemsKey: String

The key to access an array containing the added or removed web history items.

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

let WebKitErrorDomain: StringDeprecated

let WebKitErrorMIMETypeKey: StringDeprecated

let WebKitErrorPlugInNameKey: StringDeprecated

let WebKitErrorPlugInPageURLStringKey: StringDeprecated

let WebPlugInAttributesKey: String

The `NSDictionary` object containing all names and values of all attributes of the plug-in’s associated HTML element, as well as all names and values of the parameters to be passed to the plug-in. For example, this dictionary will contain all `PARAM` elements within an `APPLET` element. If attribute and parameter names conflict, the attributes of an element take precedence over any of its parameters. All keys and values in this dictionary must be of type `NSString`. *Required key*.

Deprecated

let WebPlugInBaseURLKey: String

The base URL of the document containing the plug-in’s view. *Required key*.

Deprecated

let WebPlugInContainerKey: String

An object that conforms to the `WebPlugInContainer` informal protocol. This object is used for callbacks from the plug-in to the enclosing application. If `WebPlugInContainerKey` is `nil`, no callbacks will occur.

Deprecated

let WebPlugInContainingElementKey: String

If an element of the page’s Document Object Model was used to specify the plug-in, this will contain that element. Otherwise, it will be `nil`.

Deprecated

let WebPlugInShouldLoadMainResourceKey: String

A Boolean value indicating whether the plug-in should load its own main resource (the `src` URL, in most cases).

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

static let WebViewProgressEstimateChanged: NSNotification.Name

Posted by a WebView object when the estimated progress value of a load changes.

Deprecated

static let WebViewProgressFinished: NSNotification.Name

Posted by a WebView object when the load has finished.

Deprecated

static let WebViewProgressStarted: NSNotification.Name

Posted by a WebView object when a load begins, including a load that is initiated in a subframe.

Deprecated

### Constants

let WKErrorDomain: String

String that identifies the WebKit error domain.

let WKWebsiteDataTypeFetchCache: String

let WKWebsiteDataTypeFileSystem: String

let WKWebsiteDataTypeHashSalt: String

let WKWebsiteDataTypeMediaKeys: String

let WKWebsiteDataTypeSearchFieldRecentSearches: String

let WKWebsiteDataTypeServiceWorkerRegistrations: String

## See Also

### Document Object Model (DOM) APIs

class DOMAbstractViewDeprecated

class DOMAttrDeprecated

class DOMBlobDeprecated

class DOMCDATASectionDeprecated

class DOMCharacterDataDeprecated

class DOMCommentDeprecated

class DOMCounterDeprecated

class DOMCSSCharsetRuleDeprecated

class DOMCSSFontFaceRuleDeprecated

class DOMCSSImportRuleDeprecated

class DOMCSSMediaRuleDeprecated

class DOMCSSPageRuleDeprecated

class DOMCSSPrimitiveValueDeprecated

class DOMCSSRuleDeprecated

class DOMCSSRuleListDeprecated

