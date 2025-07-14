

- IOKit
- IOKit Data Types
-  IODataQueueEntry 

Type Alias

# IODataQueueEntry

Represents an entry within the data queue

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.0+visionOS 1.0+

``` source
typealias IODataQueueEntry = _IODataQueueEntry
```

## Discussion

This is a variable sized struct. The data field simply represents the start of the data region. The size of the data region is stored in the size field. The whole size of the specific entry is the size of a UInt32 plus the size of the data region.

