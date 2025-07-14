

- WebKit
-  WKWindowFeatures 

Class

# WKWindowFeatures

Display-related attributes that a webpage requests for its window.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKWindowFeatures
```

## Overview

A WKWindowFeatures object contains the attributes that a webpage requests from its containing web view. You don’t create a WKWindowFeatures object directly. When a navigation action results in the display of a new web view, WKWebView creates this object and passes it to the webView(_:createWebViewWith:for:windowFeatures:) method of its UI delegate object. The delegate uses the information in this object to configure and return the new web view.

## Topics

### Inspecting Window Position and Dimensions

var allowsResizing: NSNumber?

A Boolean value that indicates whether to make the containing window window resizable.

var height: NSNumber?

The requested height of the containing window.

var width: NSNumber?

The requested width of the containing window.

var x: NSNumber?

The requested x-coordinate of the containing window.

var y: NSNumber?

The requested y-coordinate of the containing window.

### Inspecting Visibility Properties

var menuBarVisibility: NSNumber?

A Boolean value that indicates whether the webpage requests a visible menu bar.

var statusBarVisibility: NSNumber?

A Boolean value that indicates whether the webpage requested a visible status bar.

var toolbarsVisibility: NSNumber?

A Boolean value that indicates whether the webpage requested a visible toolbar.

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
- Sendable

## See Also

### Web View Configuration

class WKWebViewConfiguration

A collection of properties that you use to initialize a web view.

class WKProcessPool

An opaque token that you use to run multiple web views in a single process.

class WKPreferences

An object that encapsulates the standard behaviors to apply to websites.

class WKWebpagePreferences

An object that specifies the behaviors to use when loading and rendering page content.

