

- WebKit
- WKUserScript
-  injectionTime 

Instance Property

# injectionTime

The time at which to inject the script into the webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var injectionTime: WKUserScriptInjectionTime { get }
```

## Discussion

The value is one of the constants of the enumerated type WKUserScriptInjectionTime.

## See Also

### Inspecting Script Information

var source: String

The script’s source code.

enum WKUserScriptInjectionTime

Constants for the times at which to inject script content into a webpage.

var isForMainFrameOnly: Bool

A Boolean value that indicates whether to inject the script into the main frame or all frames.

