

- Foundation
- IndexPath
-  init(indexes:) 

Initializer

# init(indexes:)

Creates an index path from a sequence of integers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(indexes: ElementSequence) where ElementSequence : Sequence, ElementSequence.Element == Int
```

## See Also

### Creating Index Paths

init()

Creates an empty index path.

init(index: IndexPath.Element)

Creates an index path with a single element.

init(arrayLiteral: IndexPath.Element...)

Creates an index path from an array literal.

init(indexes: Array&lt;IndexPath.Element>)

Creates an index path from an array of elements.

