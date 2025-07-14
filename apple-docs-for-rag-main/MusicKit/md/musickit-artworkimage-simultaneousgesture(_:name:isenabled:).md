

- MusicKit
- ArtworkImage
-  simultaneousGesture(\_:name:isEnabled:) 

Instance Method

# simultaneousGesture(\_:name:isEnabled:)

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

MusicKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func simultaneousGesture(
    _ gesture: T,
    name: String,
    isEnabled: Bool = true
) -> some View where T : Gesture
```

## Parameters 

`gesture`  

A gesture to attach to the view.

`name`  

A string that identifies the gesture. In iOS, the name can be used to set up failure relationships between UIKit gesture recognizers and this gesture.

`isEnabled`  

Whether the added gesture is enabled. The default value is `true`.

## Discussion

Use this method when you need to define and process a view specific gesture simultaneously with the same priority as the view’s existing gestures. The example below defines a custom gesture that prints a message to the console and attaches it to the view’s `VStack`. Inside the `VStack` is a red heart `Image` defines its own `TapGesture` handler that also prints a message to the console and a blue rectangle with no custom gesture handlers.

You can also use the `isEnabled` parameter to conditionally disable the gesture.

Tapping or clicking the “heart” image sends two messages to the console: one for the image’s tap gesture handler, and the other from a custom gesture handler attached to the enclosing vertical stack. Tapping or clicking on the blue rectangle results only in the single message to the console from the tap recognizer attached to the `VStack`:

```
struct SimultaneousGestureExample: View {
    @State private var message = "Message"
    var isGestureEnabled: Bool
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
        .simultaneousGesture(
            newGesture, isEnabled: isGestureEnabled)
        .frame(width: 200, height: 200)
        .border(Color.purple)
    }
}
```

