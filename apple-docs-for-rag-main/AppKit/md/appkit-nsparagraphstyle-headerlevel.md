

- AppKit
- NSParagraphStyle
-  headerLevel 

Instance Property

# headerLevel

The paragraph’s header level for HTML generation.

macOS 10.0+

``` source
var headerLevel: Int { get }
```

## Discussion

If the paragraph isn’t a header, the value is `0`. If the paragraph is a header, the value ranges from `1` to `6`, depending on the header’s level.

The default value is `0`.

