

- FamilyControls
- FamilyActivityPicker
-  submitLabel(\_:) 

Instance Method

# submitLabel(\_:)

Sets the submit label for this view.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

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

## See Also

### Submission

func onSubmit(of: SubmitTriggers, () -> Void) -> some View

Adds an action to perform when the user submits a value to this view.

func submitScope(Bool) -> some View

Prevents submission triggers originating from this view to invoke a submission action configured by a submission modifier higher up in the view hierarchy.

