

- SwiftUI
- ProposedViewSize
-  replacingUnspecifiedDimensions(by:) 

Instance Method

# replacingUnspecifiedDimensions(by:)

Creates a new proposal that replaces unspecified dimensions in this proposal with the corresponding dimension of the specified size.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func replacingUnspecifiedDimensions(by size: CGSize = CGSize(width: 10, height: 10)) -> CGSize
```

## Parameters 

`size`  

A set of concrete values to use for the size proposal in place of any unspecified dimensions. The default value is `10` for both dimensions.

## Return Value

A new, fully specified size proposal.

## Discussion

Use the default value to prevent a flexible view from disappearing into a zero-sized frame, and ensure the unspecified value remains visible during debugging.

