

- RealityKit
- Model3D
-  init(named:bundle:content:placeholder:) 

Initializer

# init(named:bundle:content:placeholder:)

Loads and displays a modifiable model by name, by searching through the specified Bundle, using a custom placeholder until the model loads.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    named name: String,
    bundle: Bundle? = nil,
    @ViewBuilder content: @escaping (ResolvedModel3D) -> Model,
    @ViewBuilder placeholder: @escaping () -> Placeholder
) where Content == Model3DPlaceholderContent, Model : View, Placeholder : View
```

## Parameters 

`name`  

The name of the USD or Reality file to display.

`bundle`  

The Bundle used to look up the model by name. If not provided, defaults to the app’s main bundle.

`content`  

A closure that takes the loaded model as an input, and returns the view to show. You can return the model directly, or modify it as needed before returning it.

`placeholder`  

A closure that returns the view to show until the load operation completes successfully.

## Discussion

Until the model loads, Model3D displays the placeholder view that you specify. When the load operation completes successfully, SwiftUI updates the view to show content that you specify, which you create using the loaded model. For example, you can show a green placeholder, followed by a scaled version of the loaded model:

```
Model3D(named: "Robot-Drummer") { model in
    model.resizable()
} placeholder: {
    Color.green
}
```

If the load operation fails, Model3D continues to display the placeholder. To be able to display a different view on a load error, use the init(named:bundle:transaction:content:) initializer instead.

## See Also

### Creating a Model3D

init(named: String, bundle: Bundle?)

Loads and displays a model by name, by searching through the specified `Foundation/Bundle`.

init(named: String, bundle: Bundle?, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model by name, by searching through the specified Bundle, in phases.

init(url: URL)

Loads and displays a model from the specified URL.

init&lt;Model, Placeholder>(url: URL, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model from the specified URL using a custom placeholder until the model loads.

init(url: URL, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model from the specified URL in phases.

