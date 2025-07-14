

- GameplayKit
-  GKRTreeSplitStrategy 

Enumeration

# GKRTreeSplitStrategy

Options that control how a tree balances its internal structure when adding elements, used with the addElement(_:boundingRectMin:boundingRectMax:splitStrategy:) method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum GKRTreeSplitStrategy
```

## Topics

### Constants

case halve

An option to split groups of elements in half based on the order they were added to the tree in.

case linear

An option to split groups of elements by finding a line that divides space so that half of the elements are on either side.

case quadratic

An option to split groups of elements by finding the subgroups that occupy the least area.

case reduceOverlap

An option to split groups of elements by finding the subgroups whose areas overlap the least.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

