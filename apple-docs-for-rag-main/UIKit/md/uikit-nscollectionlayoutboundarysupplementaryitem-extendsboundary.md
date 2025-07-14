

- UIKit
- NSCollectionLayoutBoundarySupplementaryItem
-  extendsBoundary 

Instance Property

# extendsBoundary

A Boolean value that indicates whether a boundary supplementary item extends the content area of the section or layout it’s attached to.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var extendsBoundary: Bool { get set }
```

## Discussion

The default value of this property is true.

## See Also

### Specifying position

var offset: CGPoint

The floating-point value of the boundary supplementary item’s offset from the section or layout it’s attached to.

var alignment: NSRectAlignment

The alignment of the boundary supplementary item relative to the section or layout it’s attached to.

