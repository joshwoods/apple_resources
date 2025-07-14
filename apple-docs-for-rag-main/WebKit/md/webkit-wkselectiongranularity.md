

- WebKit
-  WKSelectionGranularity 

Enumeration

# WKSelectionGranularity

The granularity with which the user can select and modify web view content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum WKSelectionGranularity
```

## Topics

### Getting the Granularity Options

case dynamic

Granularity that varies automatically depending on the selection.

case character

Granularity that allows the user to place selection endpoints at any character boundary.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting selection granularity

var selectionGranularity: WKSelectionGranularity

The level of granularity with which the user can interactively select web view content.

