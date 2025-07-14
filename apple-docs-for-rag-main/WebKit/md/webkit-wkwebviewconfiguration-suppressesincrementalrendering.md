

- WebKit
- WKWebViewConfiguration
-  suppressesIncrementalRendering 

Instance Property

# suppressesIncrementalRendering

A Boolean value that indicates whether the web view suppresses content rendering until the content is fully loaded into memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var suppressesIncrementalRendering: Bool { get set }
```

## Discussion

The default value of this property is false.

## See Also

### Configuring the rendering behavior

var ignoresViewportScaleLimits: Bool

A Boolean value that determines whether a web view allows scaling of the webpage.

