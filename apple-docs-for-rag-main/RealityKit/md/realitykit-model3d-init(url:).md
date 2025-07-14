

- RealityKit
- Model3D
-  init(url:) 

Initializer

# init(url:)

Loads and displays a model from the specified URL.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(url: URL) where Content == ResolvedModel3D
```

## Parameters 

`url`  

The URL of the model to display.

## Discussion

Until the model loads, SwiftUI displays a default placeholder. When the load operation completes successfully, SwiftUI updates the view to show the loaded model. If the operation fails, SwiftUI continues to display the placeholder. The following example loads and displays a model from an example server:

```
Model3D(url: URL(string: "https://example.com/robot.usdz")!)
```

If you want to customize the placeholder or apply Model3D-specific modifiers — like `ResolvedModel3D/resizable()` — to the loaded model, use the init(url:content:placeholder:) initializer instead.

## See Also

### Creating a Model3D

init(named: String, bundle: Bundle?)

Loads and displays a model by name, by searching through the specified `Foundation/Bundle`.

init&lt;Model, Placeholder>(named: String, bundle: Bundle?, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model by name, by searching through the specified Bundle, using a custom placeholder until the model loads.

init(named: String, bundle: Bundle?, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model by name, by searching through the specified Bundle, in phases.

init&lt;Model, Placeholder>(url: URL, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model from the specified URL using a custom placeholder until the model loads.

init(url: URL, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model from the specified URL in phases.

