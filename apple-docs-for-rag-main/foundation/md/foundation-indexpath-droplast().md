

- Foundation
- IndexPath
-  dropLast() 

Instance Method

# dropLast()

Return a new index path containing all but the last element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dropLast() -> IndexPath
```

## See Also

### Selecting Nodes

func append(IndexPath)

Appends the nodes of another index path to this one.

func append(Array&lt;IndexPath.Element>)

Appends an array of elements to this index path as additional nodes.

func append(IndexPath.Element)

Appends a single element to this index path as a new node.

func appending(IndexPath.Element) -> IndexPath

Returns a new index path containing the elements of this one plus the given element.

func appending(IndexPath) -> IndexPath

Returns a new index path containing the elements of this one plus those of another index path.

func appending(Array&lt;IndexPath.Element>) -> IndexPath

Returns a new index path containing the elements of this one plus an array of additional elements.

func compare(IndexPath) -> ComparisonResult

Compares this index path to another in depth-first traversal order.

