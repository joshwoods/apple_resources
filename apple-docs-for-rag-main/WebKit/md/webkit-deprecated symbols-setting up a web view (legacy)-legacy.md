

- WebKit
- Deprecated Symbols
-  Setting Up a Web View (Legacy) 

API Collection

# Setting Up a Web View (Legacy)

## Topics

### Setting Up a Web View (Legacy)

class WebView

`WebView` is the core view class in the WebKit framework that manages interactions between the `WebFrame` and `WebFrameView` classes. To embed web content in your application, you just create a `WebView` object, attach it to a window, and send a load(_:) message to its main frame.

Deprecated

class WebPreferences

WebPreferences encapsulates the preferences you can change per WebView object. These preferences include font, text encoding, and image settings. Normally a WebView object uses the standard preferences returned by the standard() class method. However, you can modify the preferences for individual WebView instances too. Use the preferencesIdentifier WebView method to change a WebView object’s preferences, or to share preferences between WebView objects. Use the autosaves method to specify if the preferences object should be automatically saved to the user defaults database.

Deprecated

protocol WebEditingDelegateDeprecated

protocol WebUIDelegate

Web view user interface delegates implement this protocol to control the opening of new windows, augment the behavior of default menu items displayed when the user clicks elements, and perform other user interface–related tasks. These methods can be invoked as a result of handling JavaScript or other plug-in content. Delegates that display more than one web view per window, for example, need to implement some of these methods to handle that case. The default implementation assumes one window per web view, so non-conventional user interfaces might implement a user interface delegate.

Deprecated

## See Also

### WebKit Legacy APIs

Document Object Models API (Legacy)

Accessing Previous Webpages (Legacy)

Archiving Webpages (Legacy)

Loading Resources (Legacy)

Working with Frames (legacy)

Downloading Information (Legacy)

Opening a File (Legacy)

Setting Policies (Legacy)

Implementing Plugins (Legacy)

Incorporating Scripts (Legacy)

Working With Document Web Views (Legacy)

