

- RealityKit
- Model3D
-  init(named:bundle:) 

Initializer

# init(named:bundle:)

Loads and displays a model by name, by searching through the specified `Foundation/Bundle`.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    named name: String,
    bundle: Bundle? = nil
) where Content == ResolvedModel3D
```

## Parameters 

`name`  

The name of the USD or Reality file to display.

`bundle`  

The Bundle used to look up the model by name. If not provided, defaults to the app’s main bundle.

## Discussion

Until the model loads, `Model3D` displays a default placeholder. When the load operation completes successfully, `Model3D` updates the view to show the loaded model. If the operation fails, `Model3D` continues to display the placeholder. The following example loads and displays a model from an example server:

```
Model3D(named: "Robot-Drummer")
```

If you want to customize the placeholder or apply ResolvedModel3D-specific modifiers — like `ResolvedModel3D/resizable()` — to the loaded model, use the init(named:bundle:content:placeholder:) initializer instead.

## See Also

### Creating a Model3D

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

