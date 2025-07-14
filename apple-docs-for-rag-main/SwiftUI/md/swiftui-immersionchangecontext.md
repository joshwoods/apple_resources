

- SwiftUI
-  ImmersionChangeContext 

Structure

# ImmersionChangeContext

A structure that represents a state of immersion of your app.

visionOS 2.0+

``` source
struct ImmersionChangeContext
```

## Overview

You don’t use this structure directly. Instead, SwiftUI provides instances of this structure via the `onImmersionChange` modifier’s closure.

## Topics

### Instance Properties

let amount: Double?

The current amount of immersion.

## Relationships

### Conforms To

- Sendable

## See Also

### Responding to immersion changes

func onImmersionChange(initial: Bool, (ImmersionChangeContext, ImmersionChangeContext) -> Void) -> some View

Performs an action when the immersion state of your app changes.

