

- SwiftUI
- Gesture
-  map(\_:) 

Instance Method

# map(\_:)

Returns a gesture that uses the given closure to map over this gesture’s value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func map(_ body: @escaping (Self.Value) -> T) -> _MapGesture
```

