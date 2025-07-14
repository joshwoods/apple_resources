

- WebKit
- WKWebViewConfiguration
-  ignoresViewportScaleLimits 

Instance Property

# ignoresViewportScaleLimits

A Boolean value that determines whether a web view allows scaling of the webpage.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var ignoresViewportScaleLimits: Bool { get set }
```

## Discussion

When set to true, this property overrides the `user-scalable` HTML property in a webpage, and lets the web view scale its webpage content regardless of the author’s intent. The default value of this property is false.

## See Also

### Configuring the rendering behavior

var suppressesIncrementalRendering: Bool

A Boolean value that indicates whether the web view suppresses content rendering until the content is fully loaded into memory.

