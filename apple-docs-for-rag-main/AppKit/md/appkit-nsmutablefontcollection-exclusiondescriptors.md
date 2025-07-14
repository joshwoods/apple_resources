

- AppKit
- NSMutableFontCollection
-  exclusionDescriptors 

Instance Property

# exclusionDescriptors

The font descriptors to exclude from query results.

macOS 10.7+

``` source
var exclusionDescriptors: [NSFontDescriptor]? { get set }
```

## See Also

### Getting the Font Descriptors

var queryDescriptors: [NSFontDescriptor]?

The font descriptors to include in query results.

func addQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by adding the specified font descriptors.

func removeQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by removing the specified font descriptors.

