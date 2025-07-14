

- Local Authentication Embedded UI
- LAAuthenticationView
-  context 

Instance Property

# context

The local authentication context associated with the authentication view.

macOS 12.0+

``` source
@MainActor
var context: LAContext { get }
```

## See Also

### Creating a local authentication view

init(context: LAContext)

Creates a new authentication icon that reflects the current authentication state.

