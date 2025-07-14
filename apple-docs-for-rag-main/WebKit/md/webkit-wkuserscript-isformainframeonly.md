

- WebKit
- WKUserScript
-  isForMainFrameOnly 

Instance Property

# isForMainFrameOnly

A Boolean value that indicates whether to inject the script into the main frame or all frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var isForMainFrameOnly: Bool { get }
```

## Discussion

When the value of this property is true, the web view injects the script only into the main frame. When the value is false, the web view injects the script into all frames.

## See Also

### Inspecting Script Information

var source: String

The script’s source code.

var injectionTime: WKUserScriptInjectionTime

The time at which to inject the script into the webpage.

enum WKUserScriptInjectionTime

Constants for the times at which to inject script content into a webpage.

