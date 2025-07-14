

- ManagedAppDistribution
- ManagedContentView
-  gesture(\_:including:) 

Instance Method

# gesture(\_:including:)

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

ManagedAppDistributionSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func gesture(
    _ gesture: T,
    including mask: GestureMask = .all
) -> some View where T : Gesture
```

## Parameters 

`gesture`  

A gesture to attach to the view.

`mask`  

A value that controls how adding this gesture to the view affects other gestures recognized by the view and its subviews. Defaults to `SwiftUI/GestureMask/all`.

## Discussion

Use this method when you need to attach a gesture to a view. The example below defines a custom gesture that prints a message to the console and attaches it to the view’s `VStack`. Inside the `VStack` a red heart `Image` defines its own `TapGesture` handler that also prints a message to the console, and blue rectangle with no custom gesture handlers. Tapping or clicking the image prints a message to the console from the tap gesture handler on the image, while tapping or clicking the rectangle inside the `VStack` prints a message in the console from the enclosing vertical stack gesture handler.

```
struct GestureExample: View {
    @State private var message = "Message"
    let newGesture = TapGesture().onEnded {
        print("Tap on VStack.")
    }

    var body: some View {
        VStack(spacing:25) {
            Image(systemName: "heart.fill")
                .resizable()
                .frame(width: 75, height: 75)
                .padding()
                .foregroundColor(.red)
                .onTapGesture {
                    print("Tap on image.")
                }
            Rectangle()
                .fill(Color.blue)
        }
        .gesture(newGesture)
        .frame(width: 200, height: 200)
        .border(Color.purple)
    }
}
```

