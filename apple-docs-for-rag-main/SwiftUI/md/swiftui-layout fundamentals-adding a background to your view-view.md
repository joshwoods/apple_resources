

- SwiftUI
- Layout fundamentals
-  Adding a background to your view 

Article

# Adding a background to your view

Compose a background behind your view and extend it beyond the safe area insets.

## Overview

You can add a view as a background with the background(_:alignment:) view modifier. To add a background under multiple views, or to have a background larger than an existing view, you can layer the views by placing them within a ZStack, and place the view you want to be in the background at the bottom of the view stack. You can specify that a background view should ignore the safe area insets to extend the background to some or all edges.

### Add a background

If your design calls for a background, you can use the background(_:alignment:) modifier to add it underneath an existing view. The following example adds a gradient to the vertical stack using the background(_:alignment:) view modifier:

```
let backgroundGradient = LinearGradient(
    colors: [Color.red, Color.blue],
    startPoint: .top, endPoint: .bottom)

struct SignInView: View {
    @State private var name: String = ""

    var body: some View {
        VStack {
            Text("Welcome")
                .font(.title)
            HStack {
                TextField("Your name?", text: $name)
                    .textFieldStyle(.roundedBorder)
                Button(action: {}, label: {
                    Image(systemName: "arrow.right.square")
                        .font(.title)
                })
            }
            .padding()
        }
        .background(backgroundGradient)
    }
}
```

The background(_:alignment:) view modifier constrains the size of the background view to be the same size as the view to which it’s attached:

### Expand the background underneath your view

To create a background that’s larger than the vertical stack, use a different technique. You could add Spacer views above and below the content in the VStack to expand it, but that would also expand the size of the stack, possibly changing it’s layout. To add in a larger background without changing the size of the stack, nest the views within a ZStack to layer the VStack over the background view:

```
struct SignInView: View {
    @State private var name: String = ""

    var body: some View {
        ZStack {
            backgroundGradient
            VStack {
                Text("Welcome")
                    .font(.title)
                HStack {
                    TextField("Your name?", text: $name)
                        .textFieldStyle(.roundedBorder)
                    Button(action: {}, label: {
                        Image(systemName: "arrow.right.square")
                            .font(.title)
                    })
                }
                .padding()
            }
        }
    }
}
```

View sizes within a depth stack are independent, unlike when using the background view modifier. The view from Gradient expands to fill the space available to the stack, but avoids the safe area insets by default:

For more information on usings stacks to combine views, see Building layouts with stack views.

### Extend the background into the safe areas

By default, SwiftUI sizes and positions views to avoid system defined safe areas to ensure that system content or the edges of the device won’t obstruct your views. If your design calls for the background to extend to the screen edges, use the ignoresSafeArea(_:edges:) modifier to override the default.

```
struct SignInView: View {
    @State private var name: String = ""
    var body: some View {
        ZStack {
            backgroundGradient
            VStack {
                Text("Welcome")
                    .font(.title)
                HStack {
                    TextField("Your name?", text: $name)
                        .textFieldStyle(.roundedBorder)
                    Button(action: {}, label: {
                        Image(systemName: "arrow.right.square")
                            .font(.title)
                    })
                }
                .padding()
            }
        }
        .ignoresSafeArea()
    }
}
```

The background gradient fills the display area of the device and ignores the safe area insets.

### Adjust views when displaying the keyboard

You can ignore the keyboard’s safe area by adding the ignoresSafeArea(_:edges:) modifier. When you activate the keyboard, the content of the vertical stack remains fixed, ignoring the space used by the keyboard:

To get the contents of the vertical stack to respect the safe areas and adjust to the keyboard, move the modifier to only apply to the background view.

```
struct SignInView: View {
    @State private var name: String = ""
    var body: some View {
        ZStack {
            backgroundGradient
                .ignoresSafeArea()
            VStack {
                Text("Welcome")
                    .font(.title)
                HStack {
                    TextField("Your name?", text: $name)
                        .textFieldStyle(.roundedBorder)
                    Button(action: {}, label: {
                        Image(systemName: "arrow.right.square")
                            .font(.title)
                    })
                }
                .padding()
            }
        }
    }
}
```

To accommodate the keyboard, SwiftUI resizes and positions your view. Because the background view has the ignoresSafeArea(_:edges:) modifier, it remains unchanged.

## See Also

### Layering views

struct ZStack

A view that overlays its subviews, aligning them in both axes.

func zIndex(Double) -> some View

Controls the display order of overlapping views.

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background(_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

func background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

var backgroundMaterial: Material?

The material underneath the current view.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

struct ContainerBackgroundPlacement

The placement of a container background.

