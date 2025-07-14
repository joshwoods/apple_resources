

- WebKit
- WKPreferences
-  javaScriptCanOpenWindowsAutomatically 

Instance Property

# javaScriptCanOpenWindowsAutomatically

A Boolean value that indicates whether JavaScript can open windows without user interaction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var javaScriptCanOpenWindowsAutomatically: Bool { get set }
```

## Discussion

The default value is false in iOS and true in macOS.

## See Also

### Setting Java and JavaScript Preferences

var isSiteSpecificQuirksModeEnabled: Bool

A Boolean that indicates whether to apply site-specific compatibility workarounds.

