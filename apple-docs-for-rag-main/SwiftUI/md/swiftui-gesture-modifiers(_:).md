

- SwiftUI
- Gesture
-  modifiers(\_:) 

Instance Method

# modifiers(\_:)

Combines a gesture with keyboard modifiers.

macOS 10.15+

``` source
@MainActor @preconcurrency
func modifiers(_ modifiers: EventModifiers) -> _ModifiersGesture
```

## Parameters 

`modifiers`  

A set of flags that correspond to the modifier keys that the user needs to hold down.

## Return Value

A new gesture that combines a gesture with keyboard modifiers.

## Discussion

The gesture receives updates while the user presses the modifier keys that correspond to the given modifiers option set.

