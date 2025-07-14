

- SwiftUI
- VerticalAlignment
-  combineExplicit(\_:) 

Instance Method

# combineExplicit(\_:)

Merges a sequence of explicit alignment values produced by this instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func combineExplicit(_ values: S) -> CGFloat? where S : Sequence, S.Element == CGFloat?
```

## Discussion

For most alignment types, this method returns the mean of all non-`nil` values. However, some types use other rules. For example, firstTextBaseline returns the minimum value, while lastTextBaseline returns the maximum value.

## See Also

### Creating a custom alignment

init(any AlignmentID.Type)

Creates a custom vertical alignment of the specified type.

