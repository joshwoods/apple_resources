

- WebKit
- WKPreferences
-  javaScriptEnabled Deprecated

Instance Property

# javaScriptEnabled

A Boolean value that indicates whether JavaScript is enabled.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var javaScriptEnabled: Bool { get set }
```

Deprecated

Use WKWebpagePreferences.allowsContentJavaScript to disable content JavaScript on a per-navigation basis

## Discussion

The default value is true. Setting this property to false disables JavaScripts that are loaded or executed by the webpage. This setting does not affect user scripts. See WKUserContentController.

## See Also

### Deprecated

var javaEnabled: Bool

A Boolean value that indicates whether Java is enabled.

Deprecated

var plugInsEnabled: Bool

A Boolean value that indicates whether plug-ins are enabled.

Deprecated

