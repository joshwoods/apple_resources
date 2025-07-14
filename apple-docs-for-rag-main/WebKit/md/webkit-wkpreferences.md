

- WebKit
-  WKPreferences 

Class

# WKPreferences

An object that encapsulates the standard behaviors to apply to websites.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKPreferences
```

## Overview

Use a WKPreferences object to specify the preferences for your website, including the minimum font size, the JavaScript behavior, and the behavior for handling fraudulent websites. Create this object and assign it to the preferences property of the WKWebViewConfiguration object you use to create your web view.

## Topics

### Setting Rendering Preferences

var minimumFontSize: CGFloat

The minimum font size, in points.

var shouldPrintBackgrounds: Bool

A Boolean value that indicates whether to include any background color or graphics when printing content.

### Setting Behavior Preferences

var tabFocusesLinks: Bool

A Boolean value that indicates whether pressing the tab key changes the focus to links and form controls.

var isTextInteractionEnabled: Bool

A Boolean value that indicates whether to allow people to select or otherwise interact with text.

var isElementFullscreenEnabled: Bool

A Boolean value that indicates whether a web view can display content full screen.

var inactiveSchedulingPolicy: WKPreferences.InactiveSchedulingPolicy

A policy you set to specify how a web view that’s not in a window handles tasks.

enum InactiveSchedulingPolicy

An enumeration that lists policies for how a web view that’s not in a window handles tasks.

### Setting Java and JavaScript Preferences

var javaScriptCanOpenWindowsAutomatically: Bool

A Boolean value that indicates whether JavaScript can open windows without user interaction.

var isSiteSpecificQuirksModeEnabled: Bool

A Boolean that indicates whether to apply site-specific compatibility workarounds.

### Setting Fraud Warning Preferences

var isFraudulentWebsiteWarningEnabled: Bool

A Boolean value that indicates whether the web view shows warnings for suspected fraudulent content, such as malware or phishing attemps.

### Deprecated

var javaEnabled: Bool

A Boolean value that indicates whether Java is enabled.

Deprecated

var javaScriptEnabled: Bool

A Boolean value that indicates whether JavaScript is enabled.

Deprecated

var plugInsEnabled: Bool

A Boolean value that indicates whether plug-ins are enabled.

Deprecated

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
- NSSecureCoding
- Sendable

## See Also

### Web View Configuration

class WKWebViewConfiguration

A collection of properties that you use to initialize a web view.

class WKWindowFeatures

Display-related attributes that a webpage requests for its window.

class WKProcessPool

An opaque token that you use to run multiple web views in a single process.

class WKWebpagePreferences

An object that specifies the behaviors to use when loading and rendering page content.

