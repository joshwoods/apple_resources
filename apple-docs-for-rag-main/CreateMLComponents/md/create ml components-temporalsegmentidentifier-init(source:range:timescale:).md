

- Create ML Components
- TemporalSegmentIdentifier
-  init(source:range:timescale:) 

Initializer

# init(source:range:timescale:)

Creates a temporal-segment identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    source: String,
    range: Range,
    timescale: Int
)
```

## Parameters 

`source`  

A unique source description.

`range`  

A timestamp range.

`timescale`  

The number of uniquely identifiable timestamps in a second.

