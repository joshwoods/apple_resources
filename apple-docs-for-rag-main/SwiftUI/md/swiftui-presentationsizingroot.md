

- SwiftUI
-  PresentationSizingRoot 

Structure

# PresentationSizingRoot

A proxy to a view provided to the presentation with a defined presentation size.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct PresentationSizingRoot
```

## Topics

### Instance Methods

func sizeThatFits(ProposedViewSize) -> CGSize

Asks the subview for its size.

## See Also

### Adapting a presentation size

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

func presentationCompactAdaptation(PresentationAdaptation) -> some View

Specifies how to adapt a presentation to compact size classes.

struct PresentationAdaptation

Strategies for adapting a presentation to a different size class.

func presentationSizing(some PresentationSizing) -> some View

Sets the sizing of the containing presentation.

protocol PresentationSizing

A type that defines the size of the presentation content and how the presentation size adjusts to its content’s size changing.

struct PresentationSizingContext

Contextual information about a presentation.

