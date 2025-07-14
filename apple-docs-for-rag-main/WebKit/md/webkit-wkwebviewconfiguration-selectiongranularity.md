

- WebKit
- WKWebViewConfiguration
-  selectionGranularity 

Instance Property

# selectionGranularity

The level of granularity with which the user can interactively select web view content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var selectionGranularity: WKSelectionGranularity { get set }
```

## Discussion

The value is one of the constants of the enumerated type WKSelectionGranularity. The default value is WKSelectionGranularity.dynamic.

## See Also

### Setting selection granularity

enum WKSelectionGranularity

The granularity with which the user can select and modify web view content.

