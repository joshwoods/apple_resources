

- WebKit
-  WKWebViewConfiguration 

Class

# WKWebViewConfiguration

A collection of properties that you use to initialize a web view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKWebViewConfiguration
```

## Overview

A WKWebViewConfiguration object provides information about how to configure a WKWebView object. Use your configuration object to specify:

- The initial cookies to make available to your web content

- Handlers for any custom URL schemes your web content uses

- Settings for how to handle media content

- Information about how to manage selections within the web view

- Custom scripts to inject into the webpage

- Custom rules that determine how to render content

You create a WKWebViewConfiguration object in your code, configure its properties, and pass it to the initializer of your WKWebView object. The web view incorporates your configuration settings only at creation time; you cannot change those settings dynamically later.

## Topics

### Configuring the web view’s behavior

var websiteDataStore: WKWebsiteDataStore

The object you use to get and set the site’s cookies and to track the cached data objects.

var userContentController: WKUserContentController

The object that coordinates interactions between your app’s native code and the webpage’s scripts and other content.

var processPool: WKProcessPool

The object that coordinates the processes the web view uses to render its web content and execute scripts.

var applicationNameForUserAgent: String?

The app name that appears in the user agent string.

var limitsNavigationsToAppBoundDomains: Bool

A Boolean value that indicates whether the web view limits navigation to pages within the app’s domain.

var upgradeKnownHostsToHTTPS: Bool

A Boolean value that indicates whether the web view should automatically upgrade supported HTTP requests to HTTPS.

### Configuring the web view’s preferences

var preferences: WKPreferences

The object that manages the preference-related settings for the web view.

var defaultWebpagePreferences: WKWebpagePreferences!

The default preferences to use when loading and rendering content.

### Adding handlers for custom URL schemes

func setURLSchemeHandler((any WKURLSchemeHandler)?, forURLScheme: String)

Registers an object to load resources associated with the specified URL scheme.

func urlSchemeHandler(forURLScheme: String) -> (any WKURLSchemeHandler)?

Returns the currently registered handler object for the specified URL scheme.

### Configuring the rendering behavior

var ignoresViewportScaleLimits: Bool

A Boolean value that determines whether a web view allows scaling of the webpage.

var suppressesIncrementalRendering: Bool

A Boolean value that indicates whether the web view suppresses content rendering until the content is fully loaded into memory.

### Setting media playback preferences

var allowsInlineMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos play inline or use the native full-screen controller.

var allowsAirPlayForMediaPlayback: Bool

A Boolean value that indicates whether the web view allows media playback over AirPlay.

var allowsPictureInPictureMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos can play Picture in Picture.

var mediaTypesRequiringUserActionForPlayback: WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

struct WKAudiovisualMediaTypes

The media types that require a user gesture to begin playing.

### Identifying data types

var dataDetectorTypes: WKDataDetectorTypes

The types of data detectors to apply to the web view’s content.

struct WKDataDetectorTypes

The data detector types.

### Setting selection granularity

var selectionGranularity: WKSelectionGranularity

The level of granularity with which the user can interactively select web view content.

enum WKSelectionGranularity

The granularity with which the user can select and modify web view content.

### Selecting user interface directionality

var userInterfaceDirectionPolicy: WKUserInterfaceDirectionPolicy

The directionality of user interface elements.

enum WKUserInterfaceDirectionPolicy

The policy that determines the directionality of user interface elements in a web view.

### Deprecated

var mediaPlaybackAllowsAirPlay: Bool

Deprecated property.

Deprecated

var requiresUserActionForMediaPlayback: Bool

A Boolean value that indicates whether HTML5 videos require the user to start playing them (`true`) or whether the videos play automatically (`false`).

Deprecated

var mediaPlaybackRequiresUserAction: Bool

Deprecated property.

Deprecated

### Instance Properties

var allowsInlinePredictions: Bool

var supportsAdaptiveImageGlyph: Bool

var webExtensionController: WKWebExtensionController?

var writingToolsBehavior: UIWritingToolsBehavior

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Web View Configuration

class WKWindowFeatures

Display-related attributes that a webpage requests for its window.

class WKProcessPool

An opaque token that you use to run multiple web views in a single process.

class WKPreferences

An object that encapsulates the standard behaviors to apply to websites.

class WKWebpagePreferences

An object that specifies the behaviors to use when loading and rendering page content.

