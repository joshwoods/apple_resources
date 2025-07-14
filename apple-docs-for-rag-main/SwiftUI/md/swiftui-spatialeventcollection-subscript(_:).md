

- SwiftUI
- SpatialEventCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Retrieves an event using its unique identifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
subscript(index: SpatialEventCollection.Event.ID) -> SpatialEventCollection.Event? { get }
```

## Overview

Returns `nil` if the `Event` no longer exists in the collection.

## See Also

### Accessing the collection’s events

struct Event

A spatial event generated from an input like a touch or click that can drive gestures in the system.

