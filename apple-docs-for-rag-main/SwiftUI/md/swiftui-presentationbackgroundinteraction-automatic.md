

- SwiftUI
- PresentationBackgroundInteraction
-  automatic 

Type Property

# automatic

The default background interaction for the presentation.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
static var automatic: PresentationBackgroundInteraction { get }
```

## See Also

### Getting interaction types

static var disabled: PresentationBackgroundInteraction

People can’t interact with the view behind a presentation.

static var enabled: PresentationBackgroundInteraction

People can interact with the view behind a presentation.

static func enabled(upThrough: PresentationDetent) -> PresentationBackgroundInteraction

People can interact with the view behind a presentation up through a specified detent.

