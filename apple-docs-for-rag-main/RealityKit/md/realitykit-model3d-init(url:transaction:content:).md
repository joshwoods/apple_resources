

- RealityKit
- Model3D
-  init(url:transaction:content:) 

Initializer

# init(url:transaction:content:)

Loads and displays a modifiable model from the specified URL in phases.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    url: URL,
    transaction: Transaction = Transaction(),
    @ViewBuilder content: @escaping (Model3DPhase) -> Content
)
```

## Parameters 

`url`  

The URL of the image to display.

`transaction`  

The transaction to use when the phase changes.

`content`  

A closure that takes the load phase as an input, and returns the view to display for the specified phase.

## Discussion

If you set the asynchronous model’s URL to `nil`, or after you set the URL to a value but before the load operation completes, the phase is Model3DPhase.empty. After the operation completes, the phase becomes either Model3DPhase.failure(_:) or Model3DPhase.success(_:). In the first case, the phase’s error value indicates the reason for failure. In the second case, the phase’s model property contains the loaded model. Use the phase to drive the output of the `content` closure, which defines the view’s appearance:

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

To add transitions when you change the URL, apply an identifier to the Model3D.

## See Also

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

