

- AppKit
- NSTextLayoutManager
- NSTextLayoutManager.SegmentType
-  NSTextLayoutManager.SegmentType.selection 

Case

# NSTextLayoutManager.SegmentType.selection

The segment behavior suitable for selection rendering.

macOS 12.0+

``` source
case selection
```

## Discussion

This segment type extends the last segment in a line fragment to the trailing edge if continuing to the next line.

## See Also

### Kinds of text selection segments

case highlight

The segment behavior suitable for highlighting.

case standard

The standard segment, matching the typographic bounds of the range.

