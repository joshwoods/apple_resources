

- RealityKit
-  Model3D 

Structure

# Model3D

A view that asynchronously loads and displays a 3D model.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
struct Model3D where Content : View
```

## Overview

Use `Model3D` to embed a 3D model from a USD file or Reality file in your SwiftUI app.

You can use methods on the ResolvedModel3D type as well as standard view modifiers to adjust the size of the model to fit your app’s interface. Here, the resizable(_:) method scales the model to fit the current view. Then, the aspectRatio(_:contentMode:) view modifier adjusts this resizing behavior to maintain the model’s original aspect ratio, rather than scaling the `x`,` y`-, and `z` axes independently to fit the robot to the full frame of the view.

```
 Model3D(named: "Robot-Drummer") { model in
     model
         .resizable()
         .aspectRatio(contentMode: .fit)
 } placeholder: {
     ProgressView()
 }
```

If loading from a remote URL, this view uses the shared URLSession instance to load a model from the specified URL, and then display it. For example, you can display a model that’s stored on a server:

```
 Model3D(url: URL(string: "https://example.com/robot.usdz")!)
     .frame(width: 300, height: 600)
```

Until the model loads, the view displays a standard placeholder that fills the available space. After the load completes successfully, the view updates to display the model. In the example above, the model is smaller than the frame, and so appears smaller than the placeholder.

You can specify a custom placeholder using init(url:content:placeholder:). With this initializer, you can also use the `content` parameter to manipulate the loaded model. For example, you can add a modifier to make the loaded image resizable:

```
 let url = URL(string: "https://example.com/robot.usdz")!
 Model3D(url: url) { model in
     model.resizable()
 } placeholder: {
     ProgressView()
 }
 .frame(width: 50, height: 50)
```

For this example, Model3D shows a ProgressView first, and then the model scaled to fit in the specified frame:

Important

You can’t apply ResolvedModel3D-specific modifiers, like resizable(_:), directly to a `Model3D`. Instead, apply them to the `ResolvedModel3D` instance that your `content` closure gets when defining the view’s appearance.

To gain more control over the loading process, use the init(url:transaction:content:) initializer, which takes a `content` closure that receives a Model3DPhase to indicate the state of the loading operation. Return a view that’s appropriate for the current phase:

```
 let url = URL(string: "https://example.com/robot.usdz")!
 Model3D(url: url) { phase in
     if let model = phase.model {
         model // Displays the loaded model.
     } else if phase.error != nil {
         Color.red // Indicates an error.
     } else {
         Color.blue // Acts as a placeholder.
     }
 }
```

## Topics

### Creating a Model3D

init(named: String, bundle: Bundle?)

Loads and displays a model by name, by searching through the specified `Foundation/Bundle`.

init&lt;Model, Placeholder>(named: String, bundle: Bundle?, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model by name, by searching through the specified Bundle, using a custom placeholder until the model loads.

init(named: String, bundle: Bundle?, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model by name, by searching through the specified Bundle, in phases.

init(url: URL)

Loads and displays a model from the specified URL.

init&lt;Model, Placeholder>(url: URL, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model from the specified URL using a custom placeholder until the model loads.

init(url: URL, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model from the specified URL in phases.

### Accessing content

var body: some View

The content and behavior of the view.

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### SwiftUI 3D model presentation

enum Model3DPhase

The current phase of the asynchronous model loading operation.

struct ResolvedModel3D

A view for displaying static three-dimensional models.

struct Model3DPlaceholderContent

A container view that presents either a 3D model or a placeholder for one.

