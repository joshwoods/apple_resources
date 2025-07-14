

- UIKit
- UIPageControl
-  UIPageControl.InteractionState 

Enumeration

# UIPageControl.InteractionState

Constants that define the interaction states of the page control.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum InteractionState
```

## Topics

### Constants

case none

The default interaction state, where no interaction has occurred.

case discrete

The interaction state for which the page changes through a single, discrete interaction.

case continuous

The interaction state for which the page changes through a continuous interaction.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the interaction state

var allowsContinuousInteraction: Bool

A Boolean value that determines whether the page control allows continuous interaction.

var interactionState: UIPageControl.InteractionState

The interaction state when the current page changes.

