

- RealityKit
- Model3D
-  init(named:bundle:transaction:content:) 

Initializer

# init(named:bundle:transaction:content:)

Loads and displays a modifiable model by name, by searching through the specified Bundle, in phases.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    named name: String,
    bundle: Bundle? = nil,
    transaction: Transaction = Transaction(),
    @ViewBuilder content: @escaping (Model3DPhase) -> Content
)
```

## Parameters 

`name`  

The name of the USD or Reality file to display.

`bundle`  

The Bundle used to look up the model by name. If not provided, defaults to the app’s main bundle.

`transaction`  

The transaction to use when the phase changes.

`content`  

A closure that takes the load phase as an input, and returns the view to display for the specified phase.

## Discussion

Before the load operation completes, the phase is Model3DPhase.empty. After the operation completes, the phase becomes either Model3DPhase.failure(_:) or Model3DPhase.success(_:). In the first case, the phase’s error value indicates the reason for failure. In the second case, the phase’s model property contains the loaded model. Use the phase to drive the output of the `content` closure, which defines the view’s appearance:

```
    Model3D(named: "Robot-Drummer") { phase in
        if let model = phase.model {
            model // Displays the loaded model.
        } else if phase.error != nil {
            Color.red // Indicates an error.
        } else {
            Color.blue // Acts as a placeholder.
        }
    }
```

To add transitions when you change the name, apply an identifier to the Model3D.

## See Also

### Creating a Model3D

init(named: String, bundle: Bundle?)

Loads and displays a model by name, by searching through the specified `Foundation/Bundle`.

init&lt;Model, Placeholder>(named: String, bundle: Bundle?, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model by name, by searching through the specified Bundle, using a custom placeholder until the model loads.

init(url: URL)

Loads and displays a model from the specified URL.

init&lt;Model, Placeholder>(url: URL, content: (ResolvedModel3D) -> Model, placeholder: () -> Placeholder)

Loads and displays a modifiable model from the specified URL using a custom placeholder until the model loads.

init(url: URL, transaction: Transaction, content: (Model3DPhase) -> Content)

Loads and displays a modifiable model from the specified URL in phases.

