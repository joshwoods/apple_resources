

- WebKit
-  WebPreferences Deprecated

Class

# WebPreferences

WebPreferences encapsulates the preferences you can change per WebView object. These preferences include font, text encoding, and image settings. Normally a WebView object uses the standard preferences returned by the standard() class method. However, you can modify the preferences for individual WebView instances too. Use the preferencesIdentifier WebView method to change a WebView object’s preferences, or to share preferences between WebView objects. Use the autosaves method to specify if the preferences object should be automatically saved to the user defaults database.

macOS 10.3–10.14Deprecated

``` source
class WebPreferences
```

## Overview

WebPreferences also manages the font preferences for a web view. You can set custom font families for each of the primary web font styles (standard, serif, sans-serif, cursive, and fantasy) as well as their font sizes. The font size preferences alter the display font sizes in a certain way. If the HTML or CSS in the web view’s content specifies font sizes in a relative fashion (such as `font size=-1` in HTML or `font-size: medium` in CSS), the default font size settings (set by the font size methods prefaced with “default”) have an effect. They do not have an effect for font sizes specified absolutely. The values specified by the minimum font size settings (set by the font size methods prefaced with “minimum”) override all the HTML and CSS font size definitions, and so have an effect on the entirety of the content. The values specified by the minimum logical font size settings (set by the font size methods prefaced with “minimumLogical”) affect all relative font size declarations for HTML and CSS, but also override any CSS font size declarations in the content, whether they are relative or absolute.

The font size for a web view is different than its logical font size. The minimum logical font size, for example, is the absolute minimum size at which the font will display onscreen. This is meant to be a functional boundary and not a style boundary. For example, the default value for a web view’s minimum logical font size is 9 points, because typical web content looks good in macOS at font sizes of 9 point and above. The constraint assures that web content will always look good in a web view. If you know that your content will look good only at 12 points or above, you should change the minimum font size to 12 points and leave the minimum *logical* font size alone. This will assure that your content will never display at sizes less than 12 points, but the functional font size boundary of the web view will remain at 9 points to prevent any chance of displaying unnecessarily small text.

## Topics

### Getting the Standard Preferences

class func standard() -> WebPreferences!

Returns the standard set of preferences that may be used by all WebView objects.

### Initializing Preferences

init!(identifier: String!)

Returns an initialized `WebPreferences` object, creating one if it does not exist.

### Getting the Identifier

var identifier: String!

The receiver’s identifier.

### Saving Preferences to the User Defaults Database

var autosaves: Bool

A Boolean that indicates whether or not the receiver’s attributes are automatically stored in the user defaults database.

### Enabling Java

var isJavaEnabled: Bool

A Boolean that indicates whether or not the web view allows Java.

### Enabling JavaScript

var isJavaScriptEnabled: Bool

A Boolean that indicates whether or not the web view allows JavaScript.

var javaScriptCanOpenWindowsAutomatically: Bool

A Boolean that indicates whether or not the web view allows JavaScript to open windows automatically.

### Enabling Plug-ins

var arePlugInsEnabled: Bool

A Boolean that indicates whether or not the web view allows plug-ins.

### Enabling Style Sheets

var userStyleSheetEnabled: Bool

A Boolean that indicates whether or not user style sheets are enabled in the web view.

### Getting and Setting Fonts

var cursiveFontFamily: String!

The cursive font family of the web view.

var fantasyFontFamily: String!

The fantasy font family of the web view.

var fixedFontFamily: String!

The fixed font family of the web view.

var sansSerifFontFamily: String!

The sans serif font family of the web view.

var serifFontFamily: String!

The serif font family of the web view.

var standardFontFamily: String!

The standard font family of the web view.

### Getting and Setting Font Sizes

var defaultFixedFontSize: Int32

The default fixed font size of the web view.

var defaultFontSize: Int32

The default font size of the web view.

var minimumFontSize: Int32

The minimum font size of the web view.

var minimumLogicalFontSize: Int32

The minimum logical font size of the web view.

### Getting and Setting Text Encoding

var defaultTextEncodingName: String!

The default text encoding of the web view.

### Getting and Setting Incremental Rendering

var suppressesIncrementalRendering: Bool

A Boolean that indicates whether incremental rendering should be suppressed.

### Handling Images

var allowsAnimatedImageLooping: Bool

A Boolean that indicates whether or not the receiver allows animated images to loop.

var allowsAnimatedImages: Bool

A Boolean that indicates whether or not the receiver allows animated images.

var loadsImagesAutomatically: Bool

A Boolean that indicates whether or not the web view allows images to be loaded automatically.

### Printing Backgrounds

var shouldPrintBackgrounds: Bool

A Boolean that indicates whether or not the web view should include backgrounds when printing.

### Enabling Private Browsing

var privateBrowsingEnabled: Bool

A Boolean that indicates whether or not private browsing is enabled.

### Controlling User Focus

var tabsToLinks: Bool

A Boolean that indicates whether or not the tab key will focus links.

### Caching

var usesPageCache: Bool

A Boolean that indicates whether the web views associated with the receiver should use the shared page cache.

var cacheModel: WebCacheModel

The cache model for the web views associated with the receiver.

### Constants

enum WebCacheModel

Specifies the caching model for a web view.

### Notifications

static let WebPreferencesChanged: NSNotification.Name

Posted when the web preference settings are changed.

### Instance Properties

var allowsAirPlayForMediaPlayback: Bool

var userStyleSheetLocation: URL!

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Setting Up a Web View (Legacy)

class WebView

`WebView` is the core view class in the WebKit framework that manages interactions between the `WebFrame` and `WebFrameView` classes. To embed web content in your application, you just create a `WebView` object, attach it to a window, and send a load(_:) message to its main frame.

Deprecated

protocol WebEditingDelegateDeprecated

protocol WebUIDelegate

Web view user interface delegates implement this protocol to control the opening of new windows, augment the behavior of default menu items displayed when the user clicks elements, and perform other user interface–related tasks. These methods can be invoked as a result of handling JavaScript or other plug-in content. Delegates that display more than one web view per window, for example, need to implement some of these methods to handle that case. The default implementation assumes one window per web view, so non-conventional user interfaces might implement a user interface delegate.

Deprecated

