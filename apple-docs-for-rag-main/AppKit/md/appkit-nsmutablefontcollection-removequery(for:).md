

- AppKit
- NSMutableFontCollection
-  removeQuery(for:) 

Instance Method

# removeQuery(for:)

Edits the query and exclusion arrays by removing the specified font descriptors.

macOS 10.7+

``` source
func removeQuery(for descriptors: [NSFontDescriptor])
```

## Parameters 

`descriptors`  

The font descriptors to add to the query.

## See Also

### Getting the Font Descriptors

var queryDescriptors: [NSFontDescriptor]?

The font descriptors to include in query results.

func addQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by adding the specified font descriptors.

var exclusionDescriptors: [NSFontDescriptor]?

The font descriptors to exclude from query results.

