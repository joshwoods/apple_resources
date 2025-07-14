

- SwiftUI
- View
-  onSubmit(of:\_:) 

Instance Method

# onSubmit(of:\_:)

Adds an action to perform when the user submits a value to this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func onSubmit(
    of triggers: SubmitTriggers = .text,
    _ action: @escaping () -> Void
) -> some View
```

## Parameters 

`triggers`  

The triggers that should invoke the provided action.

`action`  

The action to perform on submission of a value.

## Mentioned in 

Managing search interface activation

## Discussion

Different views may have different triggers for the provided action. A TextField, or SecureField will trigger this action when the user hits the hardware or software return key. This modifier may also bind this action to a default action keyboard shortcut. You may set this action on an individual view or an entire view hierarchy.

```
TextField("Username", text: $username)
    .onSubmit {
        guard viewModel.validate() else { return }
        viewModel.login()
    }
```

You can use the submitScope(_:) modifier to stop a submit trigger from a control from propagating higher up in the view hierarchy to higher `View.onSubmit(of:_:)` modifiers.

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

You can use different submit triggers to filter the types of triggers that should invoke the provided submission action. For example, you may provide a value of search to only hear submission triggers that originate from search fields vended by searchable modifiers.

```
@StateObject private var viewModel = ViewModel()

NavigationView {
    SidebarView()
    DetailView()
}
.searchable(
    text: $viewModel.searchText,
    placement: .sidebar
) {
    SuggestionsView()
}
.onSubmit(of: .search) {
    viewModel.submitCurrentSearchQuery()
}
```

## See Also

### Responding to submission events

func submitScope(Bool) -> some View

Prevents submission triggers originating from this view to invoke a submission action configured by a submission modifier higher up in the view hierarchy.

struct SubmitTriggers

A type that defines various triggers that result in the firing of a submission action.

