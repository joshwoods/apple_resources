

- SwiftUI
-  TapGesture 

Structure

# TapGesture

A gesture that recognizes one or more taps.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 16.0+visionOS 1.0+watchOS 6.0+

``` source
struct TapGesture
```

## Overview

To recognize a tap gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:including:) modifier. The following code adds a tap gesture to a Circle that toggles the color of the circle:

```
struct TapGestureView: View {
    @State private var tapped = false

    var tap: some Gesture {
        TapGesture(count: 1)
            .onEnded { _ in self.tapped = !self.tapped }
    }

    var body: some View {
        Circle()
            .fill(self.tapped ? Color.blue : Color.red)
            .frame(width: 100, height: 100, alignment: .center)
            .gesture(tap)
    }
}
```

## Topics

### Creating a tap gesture

init(count: Int)

Creates a tap gesture with the number of required taps.

var count: Int

The required number of tap events.

## Relationships

### Conforms To

- Gesture

## See Also

### Recognizing tap gestures

func onTapGesture(count: Int, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture.

func onTapGesture(count:coordinateSpace:perform:)

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

struct SpatialTapGesture

A gesture that recognizes one or more taps and reports their location.

