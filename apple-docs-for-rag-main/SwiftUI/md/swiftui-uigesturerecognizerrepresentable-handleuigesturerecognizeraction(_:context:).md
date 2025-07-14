

- SwiftUI
- UIGestureRecognizerRepresentable
-  handleUIGestureRecognizerAction(\_:context:) 

Instance Method

# handleUIGestureRecognizerAction(\_:context:)

Handles recognition of the represented `UIGestureRecognizer`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func handleUIGestureRecognizerAction(
    _ recognizer: Self.UIGestureRecognizerType,
    context: Self.Context
)
```

**Required** Default implementation provided.

## Parameters 

`recognizer`  

An instance of the represented gesture recognizer.

`context`  

A context structure containing information about the current state of the system, such as the current coordinator instance.

## Discussion

If you implement this method, SwiftUI calls it when the wrapped gesture recognizer is recognized.

## Default Implementations

### UIGestureRecognizerRepresentable Implementations

func handleUIGestureRecognizerAction(Self.UIGestureRecognizerType, context: Self.Context)

Handles recognition of the represented `UIGestureRecognizer`.

