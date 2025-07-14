

- UIKit
- UIBandSelectionInteraction
-  UIBandSelectionInteraction.State 

Enumeration

# UIBandSelectionInteraction.State

Constants that indicate whether a band selection interaction object is inactive or currently tracking an interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
enum State
```

## Overview

Use the UIBandSelectionInteraction.State constants in the handler of a UIBandSelectionInteraction object to determine the current state of the interaction. When the interaction object is idle, it sets the state to UIBandSelectionInteraction.State.possible. After the interaction starts, the state changes to other values to reflect the progress toward the completion of that interaction.

## Topics

### Getting the selection state

case possible

A state that indicates the interaction object is ready to start a new interaction.

case began

A state that indicates the interaction object began a new interaction.

case selecting

A state that indicates the interaction object is tracking changes to the selection rectangle.

case ended

A state that indicates the current interaction ended.

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

### Band selection

class UIBandSelectionInteraction

An object that tracks the selection of multiple items using pointer-based input.

