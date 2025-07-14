

- Local Authentication Embedded UI
- LAAuthenticationView
-  controlSize 

Instance Property

# controlSize

The size of the local authentication view user interface element.

macOS 12.0+

``` source
@MainActor
var controlSize: NSControl.ControlSize { get }
```

## See Also

### Controlling the size of a local authentication view

init(context: LAContext, controlSize: NSControl.ControlSize)

Creates a new authentication icon that reflects the current authentication state, using a specified size.

