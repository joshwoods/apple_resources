

- AppKit
- NSTextSelection
-  init(coder:) 

Initializer

# init(coder:)

Creates a test selection from data in an unarchiver.

macOS 12.0+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

A coder that subclasses NSCoder.

## See Also

### Creating a text selection

convenience init(any NSTextLocation, affinity: NSTextSelection.Affinity)

Creates a new text selection with the location and selection affinity you provide.

convenience init(range: NSTextRange, affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the range, selection affinity, and granularity you provide.

init([NSTextRange], affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the ranges, selection affinity, and granularity you provide.

