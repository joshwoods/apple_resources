

- SwiftUI
- ProposedViewSize
-  infinity 

Type Property

# infinity

A size proposal that contains infinity in both dimensions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let infinity: ProposedViewSize
```

## Discussion

Both dimensions contain doc://com.apple.documentation/documentation/CoreFoundation/CGFloat/1454161-infinity in this size proposal. Subviews of a custom layout return their maximum size when you propose this value using the dimensions(in:) method. A custom layout should also return its maximum size from the sizeThatFits(proposal:subviews:cache:) method for this value.

## See Also

### Getting standard proposals

static let zero: ProposedViewSize

A size proposal that contains zero in both dimensions.

static let unspecified: ProposedViewSize

The proposed size with both dimensions left unspecified.

