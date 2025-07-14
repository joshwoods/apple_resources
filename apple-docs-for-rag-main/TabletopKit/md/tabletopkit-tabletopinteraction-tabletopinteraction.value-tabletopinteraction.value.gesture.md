

- TabletopKit
- TabletopInteraction
- TabletopInteraction.Value
-  TabletopInteraction.Value.Gesture 

Structure

# TabletopInteraction.Value.Gesture

A structure that provides details specific to a gesture driven interaction.

visionOS 2.2+

``` source
struct Gesture
```

## Topics

### Instance Properties

var chirality: TabletopInteraction.Value.Gesture.Chirality?

The chirality, or handedness, of this gesture, if known.

var kind: TabletopInteraction.Value.Gesture.Kind

The input source or mode which started this gesture.

var phase: TabletopInteraction.Value.Phase

The current phase of the gesture.

### Enumerations

enum Chirality

The chirality, or handedness, of a gesture.

enum Kind

The possible input sources or modes that can start a gesture interaction.

## Relationships

### Conforms To

- Sendable

