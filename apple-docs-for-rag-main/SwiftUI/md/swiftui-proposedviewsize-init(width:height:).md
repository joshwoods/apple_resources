

- SwiftUI
- ProposedViewSize
-  init(width:height:) 

Initializer

# init(width:height:)

Creates a new proposed size using the specified width and height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    width: CGFloat?,
    height: CGFloat?
)
```

## Parameters 

`width`  

A proposed width in points. Use a value of `nil` to indicate that the width is unspecified for this proposal.

`height`  

A proposed height in points. Use a value of `nil` to indicate that the height is unspecified for this proposal.

## See Also

### Creating a custom size proposal

init(CGSize)

Creates a new proposed size from a specified size.

