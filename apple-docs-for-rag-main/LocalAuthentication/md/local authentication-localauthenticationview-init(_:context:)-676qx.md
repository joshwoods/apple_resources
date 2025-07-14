

- Local Authentication
- LocalAuthenticationView
-  init(\_:context:) 

Initializer

# init(\_:context:)

Creates a local authentication view with a localizable title and required context.

LocalAuthenticationSwiftUImacOS 13.0+

``` source
@MainActor @preconcurrency
init(
    _ titleKey: LocalizedStringKey,
    context: LAContext
) where Label == Text
```

## Parameters 

`titleKey`  

A localized title that displays below the authentication view.

`context`  

A context used to evaluate authentication policies.

## See Also

### Authenticating with a context you supply

init&lt;S>(S, context: LAContext)

Creates a local authentication view with a required context.

init(context: LAContext, label: () -> Label)

Creates a local authentication view with a label and required context.

