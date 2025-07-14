

- UIKit
- NSTextSelection
-  init(\_:affinity:granularity:) 

Initializer

# init(\_:affinity:granularity:)

Creates a new text selection with the ranges, selection affinity, and granularity you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    _ textRanges: [NSTextRange],
    affinity: NSTextSelection.Affinity,
    granularity: NSTextSelection.Granularity
)
```

## Parameters 

`textRanges`  

An array of text ranges.

`affinity`  

One of the available NSTextSelection.Affinity options.

`granularity`  

One of the available NSTextSelection.Granularity options.

## See Also

### Creating a text selection

convenience init(any NSTextLocation, affinity: NSTextSelection.Affinity)

Creates a new text selection with the location and selection affinity you provide.

convenience init(range: NSTextRange, affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the range, selection affinity, and granularity you provide.

init?(coder: NSCoder)

Creates a test selection from data in an unarchiver.

