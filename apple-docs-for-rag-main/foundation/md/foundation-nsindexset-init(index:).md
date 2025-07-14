

- Foundation
- NSIndexSet
-  init(index:) 

Initializer

# init(index:)

Initializes an allocated NSIndexSet object with an index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(index value: Int)
```

## Parameters 

`value`  

An index. Must be in the range `0 .. NSNotFound - 1`.

## Return Value

Initialized NSIndexSet object with `index`.

## See Also

### Creating Index Sets

init(indexesIn: NSRange)

Initializes an allocated NSIndexSet object with an index range.

init(indexSet: IndexSet)

Initializes an allocated NSIndexSet object with an index set.

