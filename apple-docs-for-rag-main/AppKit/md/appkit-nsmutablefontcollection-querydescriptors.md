

- AppKit
- NSMutableFontCollection
-  queryDescriptors 

Instance Property

# queryDescriptors

The font descriptors to include in query results.

macOS 10.7+

``` source
var queryDescriptors: [NSFontDescriptor]? { get set }
```

## See Also

### Getting the Font Descriptors

func addQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by adding the specified font descriptors.

func removeQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by removing the specified font descriptors.

var exclusionDescriptors: [NSFontDescriptor]?

The font descriptors to exclude from query results.

