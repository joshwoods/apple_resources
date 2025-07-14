

- SwiftUI
-  SpatialTapGesture 

Structure

# SpatialTapGesture

A gesture that recognizes one or more taps and reports their location.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
struct SpatialTapGesture
```

## Overview

To recognize a tap gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:including:) modifier. The following code adds a tap gesture to a Circle that toggles the color of the circle based on the tap location:

```
struct TapGestureView: View {
    @State private var location: CGPoint = .zero

    var tap: some Gesture {
        SpatialTapGesture()
            .onEnded { event in
                self.location = event.location
             }
    }

    var body: some View {
        Circle()
            .fill(self.location.y > 50 ? Color.blue : Color.red)
            .frame(width: 100, height: 100, alignment: .center)
            .gesture(tap)
    }
}
```

## Topics

### Creating a spatial tap gesture

init(count: Int, coordinateSpace: some CoordinateSpaceProtocol)

Creates a tap gesture with the number of required taps and the coordinate space of the gesture’s location.

var coordinateSpace: CoordinateSpace

The coordinate space in which to receive location values.

var count: Int

The required number of tap events.

### Getting the gesture’s value

struct Value

The attributes of a tap gesture.

### Deprecated initializers

init(count: Int, coordinateSpace: CoordinateSpace)

Creates a tap gesture with the number of required taps and the coordinate space of the gesture’s location.

Deprecated

### Initializers

init(count:coordinateSpace:)

Creates a tap gesture with the number of required taps and the coordinate space of the gesture’s location.

## Relationships

### Conforms To

- Gesture

## See Also

### Recognizing tap gestures

func onTapGesture(count: Int, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture.

func onTapGesture(count:coordinateSpace:perform:)

Adds an action to perform when this view recognizes a tap gesture, and provides the action with the location of the interaction.

struct TapGesture

A gesture that recognizes one or more taps.

