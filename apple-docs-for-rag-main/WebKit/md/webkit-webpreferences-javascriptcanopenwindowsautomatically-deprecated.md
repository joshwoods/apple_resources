

- WebKit
- WebPreferences
-  javaScriptCanOpenWindowsAutomatically Deprecated

Instance Property

# javaScriptCanOpenWindowsAutomatically

A Boolean that indicates whether or not the web view allows JavaScript to open windows automatically.

macOS 10.3–10.14Deprecated

``` source
var javaScriptCanOpenWindowsAutomatically: Bool { get set }
```

## Discussion

Set to true if the web view should allow JavaScript to open windows automatically, otherwise false.

Explicit calls to a JavaScript window opener that are activated by user action (such as a button click) are not affected by this setting.

## See Also

### Enabling JavaScript

var isJavaScriptEnabled: Bool

A Boolean that indicates whether or not the web view allows JavaScript.

Deprecated

