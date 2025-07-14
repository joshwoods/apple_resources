

- Local Authentication
- LocalAuthenticationView
-  init(context:label:) 

Initializer

# init(context:label:)

Creates a local authentication view with a label and required context.

LocalAuthenticationSwiftUImacOS 13.0+

``` source
@MainActor @preconcurrency
init(
    context: LAContext,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`context`  

A context used to evaluate authentication policies.

`label`  

A label that displays below the authentication view.

## See Also

### Authenticating with a context you supply

init&lt;S>(S, context: LAContext)

Creates a local authentication view with a required context.

init(LocalizedStringKey, context: LAContext)

Creates a local authentication view with a localizable title and required context.

