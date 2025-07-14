

- UIKit
- NSTextSelection
-  init(\_:affinity:) 

Initializer

# init(\_:affinity:)

Creates a new text selection with the location and selection affinity you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init(
    _ location: any NSTextLocation,
    affinity: NSTextSelection.Affinity
)
```

## Parameters 

`location`  

The text location

`affinity`  

One of the possible NSTextSelection.Affinity options.

## See Also

### Creating a text selection

convenience init(range: NSTextRange, affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the range, selection affinity, and granularity you provide.

init([NSTextRange], affinity: NSTextSelection.Affinity, granularity: NSTextSelection.Granularity)

Creates a new text selection with the ranges, selection affinity, and granularity you provide.

init?(coder: NSCoder)

Creates a test selection from data in an unarchiver.

