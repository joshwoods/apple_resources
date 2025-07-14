

- WebKit
-  WKWebpagePreferences 

Class

# WKWebpagePreferences

An object that specifies the behaviors to use when loading and rendering page content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
@MainActor
class WKWebpagePreferences
```

## Overview

Create a WKWebpagePreferences object when you want to change the default rendering behavior of your web view. Typically, iOS devices render web content for a mobile experience, and Mac devices render content for a desktop experience.

## Topics

### Setting the JavaScript preferences

var allowsContentJavaScript: Bool

A Boolean value that indicates whether JavaScript from web content is allowed to run.

### Setting the preferred content mode

var preferredContentMode: WKWebpagePreferences.ContentMode

The content mode for the web view to use when it loads and renders a webpage.

enum ContentMode

Constants that indicate how to render web view content.

### Getting Lockdown Mode info

var isLockdownModeEnabled: Bool

A Boolean value that indicates whether to use Lockdown Mode in the web view.

### Instance Properties

var preferredHTTPSNavigationPolicy: WKWebpagePreferences.UpgradeToHTTPSPolicy

### Enumerations

enum UpgradeToHTTPSPolicy

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

class WKWindowFeatures

Display-related attributes that a webpage requests for its window.

class WKProcessPool

An opaque token that you use to run multiple web views in a single process.

class WKPreferences

An object that encapsulates the standard behaviors to apply to websites.

