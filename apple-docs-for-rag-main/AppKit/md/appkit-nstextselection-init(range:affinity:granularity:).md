

- AppKit
- NSTextSelection
-  init(range:affinity:granularity:) 

Initializer

# init(range:affinity:granularity:)

Creates a new text selection with the range, selection affinity, and granularity you provide.

macOS 12.0+

``` source
convenience init(
    range: NSTextRange,
    affinity: NSTextSelection.Affinity,
    granularity: NSTextSelection.Granularity
)
```

## Parameters 

`range`  

The range of the selection.

`affinity`  

One of the available NSTextSelection.Affinity options.

`granularity`  

One of the available NSTextSelection.Granularity options.

## See Also

### Creating a text selection

convenience init(any NSTextLocation, affinity: NSTextSelection.Affinity)

Creates a new text selection with the location and selection affinity you provide.

init([NSTextRange], affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the ranges, selection affinity, and granularity you provide.

init?(coder: NSCoder)

Creates a test selection from data in an unarchiver.

