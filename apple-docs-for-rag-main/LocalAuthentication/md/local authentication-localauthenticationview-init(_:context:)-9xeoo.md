

- Local Authentication
- LocalAuthenticationView
-  init(\_:context:) 

Initializer

# init(\_:context:)

Creates a local authentication view with a required context.

LocalAuthenticationSwiftUImacOS 13.0+

``` source
@MainActor @preconcurrency
init(
    _ title: S,
    context: LAContext
) where Label == Text, S : StringProtocol
```

## Parameters 

`title`  

A title that displays below the authentication view.

`context`  

A context used to evaluate authentication policies.

## See Also

### Authenticating with a context you supply

init(context: LAContext, label: () -> Label)

Creates a local authentication view with a label and required context.

init(LocalizedStringKey, context: LAContext)

Creates a local authentication view with a localizable title and required context.

