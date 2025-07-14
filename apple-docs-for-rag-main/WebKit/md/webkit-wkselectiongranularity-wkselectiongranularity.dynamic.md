

- WebKit
- WKSelectionGranularity
-  WKSelectionGranularity.dynamic 

Case

# WKSelectionGranularity.dynamic

Granularity that varies automatically depending on the selection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case dynamic
```

## Discussion

When the selection is within a single block, the granularity may be single character. When the selection is not confined to a single block, the granularity may be a single block.

## See Also

### Getting the Granularity Options

case character

Granularity that allows the user to place selection endpoints at any character boundary.

