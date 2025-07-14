

- Local Authentication
- LocalAuthenticationView
-  init(\_:reason:context:result:) 

Initializer

# init(\_:reason:context:result:)

Creates a local authentication view with a title.

LocalAuthenticationSwiftUImacOS 13.0+

``` source
@MainActor @preconcurrency
init(
    _ title: S,
    reason: Text,
    context: LAContext? = nil,
    result: @escaping (Result) -> Void
) where Label == Text, S : StringProtocol
```

## Parameters 

`title`  

A title that displays below the authentication view.

`reason`  

A localized reason that describes why your app presents an authentication prompt to the user.

`context`  

A context used to evaluate authentication policies. If `nil`, the system creates one.

`result`  

A closure to call when the authentication succeeds or fails.

`result`  
A Result instance that indicates success or failure with a reason.

## See Also

### Authenticating with an implicit context

init(reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void, label: () -> Label)

Creates a local authentication view.

init(LocalizedStringKey, reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void)

Creates a local authentication view with a localizable title.

init(Text, reason: Text, context: LAContext?, result: (Result&lt;Void, any Error>) -> Void)

Creates a local authentication view with a title text view.

