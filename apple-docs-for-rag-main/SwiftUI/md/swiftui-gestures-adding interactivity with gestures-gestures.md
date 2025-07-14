

- SwiftUI
- Gestures
-  Adding interactivity with gestures 

Article

# Adding interactivity with gestures

Use gesture modifiers to add interactivity to your app.

## Overview

Gesture modifiers handle all of the logic needed to process user-input events such as touches, and recognize when those events match a known gesture pattern, such as a long press or rotation. When recognizing a pattern, SwiftUI runs a callback you use to update the state of a view or perform an action.

### Add gesture modifiers to a view

Each gesture you add applies to a specific view in the view hierarchy. To recognize a gesture event on a particular view, create and configure the gesture, and then use the gesture(_:including:) modifier:

```
struct ShapeTapView: View {
    var body: some View {
        let tap = TapGesture()
            .onEnded { _ in
                print("View tapped!")
            }

        return Circle()
            .fill(Color.blue)
            .frame(width: 100, height: 100, alignment: .center)
            .gesture(tap)
    }
}
```

### Respond to gesture callbacks

Depending on the callbacks you add to a gesture modifier, SwiftUI reports back to your code whenever the state of the gesture changes. Gesture modifiers offer three ways to receive updates: updating(_:body:), onChanged(_:), and onEnded(_:).

#### Update transient UI state

To update a view as a gesture changes, add a GestureState property to your view and update it in the updating(_:body:) callback. SwiftUI invokes the updating callback as soon as it recognizes the gesture and whenever the value of the gesture changes. For example, SwiftUI invokes the updating callback as soon as a magnification gesture begins and then again whenever the magnification value changes. SwiftUI doesn’t invoke the updating callback when the user ends or cancels a gesture. Instead, the gesture state property automatically resets its state back to its initial value.

For example, to make a view that changes color while the user performs a long press, add a gesture state property and update it in the updating callback.

```
struct CounterView: View {
    @GestureState private var isDetectingLongPress = false

    var body: some View {
        let press = LongPressGesture(minimumDuration: 1)
            .updating($isDetectingLongPress) { currentState, gestureState, transaction in
                gestureState = currentState
            }

        return Circle()
            .fill(isDetectingLongPress ? Color.yellow : Color.green)
            .frame(width: 100, height: 100, alignment: .center)
            .gesture(press)
    }
}
```

#### Update permanent state during a gesture

To track changes to a gesture that shouldn’t reset once the gesture ends, use the onChanged(_:) callback. For example, to count the number of times your app recognizes a long press, add an onChanged(_:) callback and increment a counter.

```
struct CounterView: View {
    @GestureState private var isDetectingLongPress = false
    @State private var totalNumberOfTaps = 0

    var body: some View {
        let press = LongPressGesture(minimumDuration: 1)
            .updating($isDetectingLongPress) { currentState, gestureState, transaction in
                gestureState = currentState
            }.onChanged { _ in
                self.totalNumberOfTaps += 1
            }

        return VStack {
            Text("\(totalNumberOfTaps)")
                .font(.largeTitle)

            Circle()
                .fill(isDetectingLongPress ? Color.yellow : Color.green)
                .frame(width: 100, height: 100, alignment: .center)
                .gesture(press)
        }
    }
}
```

#### Update permanent state when a gesture ends

To recognize when a gesture successfully completes and to retrieve the gesture’s final value, use the onEnded(_:) function to update your app’s state in the callback. SwiftUI only invokes the onEnded(_:) callback when the gesture succeeds. For example, during a LongPressGesture if the user stops touching the view before minimumDuration seconds have elapsed or moves their finger more than maximumDistance points SwiftUI does not invoke the onEnded(_:) callback.

For example, to stop counting long press attempts after the user completes a long press, add an onEnded(_:) callback and conditionally apply the gesture modifier.

```
struct CounterView: View {
    @GestureState private var isDetectingLongPress = false
    @State private var totalNumberOfTaps = 0
    @State private var doneCounting = false

    var body: some View {
        let press = LongPressGesture(minimumDuration: 1)
            .updating($isDetectingLongPress) { currentState, gestureState, transaction in
                gestureState = currentState
            }.onChanged { _ in
                self.totalNumberOfTaps += 1
            }
            .onEnded { _ in
                self.doneCounting = true
            }

        return VStack {
            Text("\(totalNumberOfTaps)")
                .font(.largeTitle)

            Circle()
                .fill(doneCounting ? Color.red : isDetectingLongPress ? Color.yellow : Color.green)
                .frame(width: 100, height: 100, alignment: .center)
                .gesture(doneCounting ? nil : press)
        }
    }
}
```

