

- SwiftUI
-  UIGestureRecognizerRepresentable 

Protocol

# UIGestureRecognizerRepresentable

A wrapper for a `UIGestureRecognizer` that you use to integrate that gesture recognizer into your SwiftUI hierarchy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
protocol UIGestureRecognizerRepresentable
```

## Overview

Use a UIGestureRecognizerRepresentable instance to create and manage a UIGestureRecognizer object in your SwiftUI interface.

To add your gesture recognizer to a SwiftUI view, create an instance of UIGestureRecognizerRepresentable and use the gesture(_:) modifier to attach it. The system calls the methods of your representable instance at appropriate times to create and update the gesture recognizer.

The following example shows the inclusion of a custom `MyGestureRecognizer` structure in the view hierarchy.

```
struct ContentView: View {
   var body: some View {
      VStack {
         Image("Mountain").gesture(MyGestureRecognizer())
      }
   }
}
```

Because your UIGestureRecognizerRepresentable is a struct, it can use the environment, have data dependencies, and is more similar to views in SwiftUI. The system will call the appropriate methods on your instance to propagate the latest data.

## Handling Gesture Recognizer Actions

SwiftUI automatically installs a target to handle the gesture recognizer’s action on your behalf. Implement the `handleUIGestureRecognizerAction` method to react to the gesture recognizing its action.

You can optionally include a coordinator object to forward delegate messages from your gesture recognizer or add additional targets.

## Coordinate Space Conversions

The gesture recognizer you create may not be attached to a UIView in the hierarchy, or it may return a view with different geometry than your SwiftUI view.

To handle this, use the converter on the context to perform coordinate space conversions from the global coordinate space. You can pass the gesture recognizer and a SwiftUI coordinate space to the converter to retrieve a final converted point. Passing the local coordinate space (the default) will provide the point in the SwiftUI view the gesture recognizer is attached to.

## Topics

### Associated Types

associatedtype Coordinator = Void

A type to coordinate with the gesture recognizer.

**Required**

associatedtype UIGestureRecognizerType : UIGestureRecognizer

The type of `UIGestureRecognizer` to be presented.

**Required**

### Instance Methods

func handleUIGestureRecognizerAction(Self.UIGestureRecognizerType, context: Self.Context)

Handles recognition of the represented `UIGestureRecognizer`.

**Required** Default implementation provided.

func makeCoordinator(converter: Self.CoordinateSpaceConverter) -> Self.Coordinator

Creates the custom object that you use to communicate state changes from your gesture recognizer to other parts of your SwiftUI interface.

**Required** Default implementation provided.

func makeUIGestureRecognizer(context: Self.Context) -> Self.UIGestureRecognizerType

Creates an instance of the represented gesture recognizer.

**Required**

func updateUIGestureRecognizer(Self.UIGestureRecognizerType, context: Self.Context)

Updates the `UIGestureRecognizer` (and coordinator) to the latest configuration.

**Required** Default implementation provided.

### Type Aliases

typealias Context

Contextual information about the state of the system that you use to create and update your gesture recognizer.

typealias CoordinateSpaceConverter

A type used to convert coordinates to/from coordinate spaces in the hierarchy of the associated SwiftUI view.

## See Also

### Integrate gesture recognizer into SwiftUI view hierarchies

struct UIGestureRecognizerRepresentableContext

Contextual information about the state of the system that you use to create and update a represented gesture recognizer.

struct UIGestureRecognizerRepresentableCoordinateSpaceConverter

A proxy structure used to convert locations to/from coordinate spaces in the hierarchy of the SwiftUI view associated with a UIGestureRecognizerRepresentable.

