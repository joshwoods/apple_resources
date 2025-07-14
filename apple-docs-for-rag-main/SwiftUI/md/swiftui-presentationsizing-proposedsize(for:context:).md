

- SwiftUI
- PresentationSizing
-  proposedSize(for:context:) 

Instance Method

# proposedSize(for:context:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func proposedSize(
    for root: PresentationSizingRoot,
    context: PresentationSizingContext
) -> ProposedViewSize
```

**Required**

## See Also

### Creating custom presentation size

func fitted(horizontal: Bool, vertical: Bool) -> some PresentationSizing

func sticky(horizontal: Bool, vertical: Bool) -> some PresentationSizing

Modifies self to be sticky in the specified dimensions — growing, but not shrinking.

