

- SwiftUI
- View
-  simultaneousGesture(\_:including:) 

Instance Method

# simultaneousGesture(\_:including:)

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func simultaneousGesture(
    _ gesture: T,
    including mask: GestureMask = .all
) -> some View where T : Gesture
```

## Parameters 

`gesture`  

A gesture to attach to the view.

`mask`  

A value that controls how adding this gesture to the view affects other gestures recognized by the view and its subviews. Defaults to all.

## Discussion

Use this method when you need to define and process a view specific gesture simultaneously with the same priority as the view’s existing gestures. The example below defines a custom gesture that prints a message to the console and attaches it to the view’s VStack. Inside the VStack is a red heart Image defines its own TapGesture handler that also prints a message to the console and a blue rectangle with no custom gesture handlers.

Tapping or clicking the “heart” image sends two messages to the console: one for the image’s tap gesture handler, and the other from a custom gesture handler attached to the enclosing vertical stack. Tapping or clicking on the blue rectangle results only in the single message to the console from the tap recognizer attached to the VStack:

```
struct SimultaneousGestureExample: View {
    @State private var message = "Message"
    let newGesture = TapGesture().onEnded {
        print("Gesture on VStack.")
    }

    var body: some View {
        VStack(spacing:25) {
            Image(systemName: "heart.fill")
                .resizable()
                .frame(width: 75, height: 75)
                .padding()
                .foregroundColor(.red)
                .onTapGesture {
                    print("Gesture on image.")
                }
            Rectangle()
                .fill(Color.blue)
        }
        .simultaneousGesture(newGesture)
        .frame(width: 200, height: 200)
        .border(Color.purple)
    }
}
```

## See Also

### Combining gestures

Composing SwiftUI gestures

Combine gestures to create complex interactions.

func simultaneousGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

struct SequenceGesture

A gesture that’s a sequence of two gestures.

struct SimultaneousGesture

A gesture containing two gestures that can happen at the same time with neither of them preceding the other.

struct ExclusiveGesture

A gesture that consists of two gestures where only one of them can succeed.

