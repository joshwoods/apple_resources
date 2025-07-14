

- SwiftUI
- PresentationSizing
-  fitted(horizontal:vertical:) 

Instance Method

# fitted(horizontal:vertical:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func fitted(
    horizontal: Bool,
    vertical: Bool
) -> some PresentationSizing
```

## See Also

### Creating custom presentation size

func proposedSize(for: PresentationSizingRoot, context: PresentationSizingContext) -> ProposedViewSize

**Required**

func sticky(horizontal: Bool, vertical: Bool) -> some PresentationSizing

Modifies self to be sticky in the specified dimensions — growing, but not shrinking.

