

- RealityKit
- RealityView
-  submitLabel(\_:) 

Instance Method

# submitLabel(\_:)

Sets the submit label for this view.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func submitLabel(_ submitLabel: SubmitLabel) -> some View
```

## Parameters 

`submitLabel`  

One of the cases specified in `SubmitLabel`.

## Discussion

```
Form {
    TextField("Username", $viewModel.username)
        .submitLabel(.continue)
    SecureField("Password", $viewModel.password)
        .submitLabel(.done)
}
```

