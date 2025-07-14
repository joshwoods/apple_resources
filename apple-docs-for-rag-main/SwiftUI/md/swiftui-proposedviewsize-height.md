

- SwiftUI
- ProposedViewSize
-  height 

Instance Property

# height

The proposed vertical size measured in points.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var height: CGFloat?
```

## Discussion

A value of `nil` represents an unspecified height proposal, which a view interprets to mean that it should use its ideal height.

## See Also

### Getting the proposal’s dimensions

var width: CGFloat?

The proposed horizontal size measured in points.

