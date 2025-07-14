

- Foundation
- SortDescriptor
-  init(\_:comparator:order:) 

Initializer

# init(\_:comparator:order:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ keyPath: any KeyPath & Sendable,
    comparator: String.StandardComparator = .localizedStandard,
    order: SortOrder
) where Compared : NSObject
```

