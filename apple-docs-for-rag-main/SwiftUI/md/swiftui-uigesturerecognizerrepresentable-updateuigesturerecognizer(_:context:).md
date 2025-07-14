

- SwiftUI
- UIGestureRecognizerRepresentable
-  updateUIGestureRecognizer(\_:context:) 

Instance Method

# updateUIGestureRecognizer(\_:context:)

Updates the `UIGestureRecognizer` (and coordinator) to the latest configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
func updateUIGestureRecognizer(
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

## Default Implementations

### UIGestureRecognizerRepresentable Implementations

func updateUIGestureRecognizer(Self.UIGestureRecognizerType, context: Self.Context)

Updates the `UIGestureRecognizer` (and coordinator) to the latest configuration.

