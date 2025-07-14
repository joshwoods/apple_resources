

- SwiftUI
- View
-  submitScope(\_:) 

Instance Method

# submitScope(\_:)

Prevents submission triggers originating from this view to invoke a submission action configured by a submission modifier higher up in the view hierarchy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func submitScope(_ isBlocking: Bool = true) -> some View
```

## Parameters 

`isBlocking`  

A Boolean that indicates whether this scope is actively blocking submission triggers from reaching higher submission actions.

## Discussion

Use this modifier when you want to avoid specific views from initiating a submission action configured by the onSubmit(of:_:) modifier. In the example below, the tag field doesn’t trigger the submission of the form:

```
Form {
    TextField("Username", text: $viewModel.userName)
    SecureField("Password", text: $viewModel.password)

    TextField("Tags", text: $viewModel.tags)
        .submitScope()
}
.onSubmit {
    guard viewModel.validate() else { return }
    viewModel.login()
}
```

## See Also

### Responding to submission events

func onSubmit(of: SubmitTriggers, () -> Void) -> some View

Adds an action to perform when the user submits a value to this view.

struct SubmitTriggers

A type that defines various triggers that result in the firing of a submission action.

