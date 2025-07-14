

- Local Authentication Embedded UI
- LAAuthenticationView
-  init(context:controlSize:) 

Initializer

# init(context:controlSize:)

Creates a new authentication icon that reflects the current authentication state, using a specified size.

macOS 12.0+

``` source
@MainActor
init(
    context: LAContext,
    controlSize: NSControl.ControlSize
)
```

## Parameters 

`context`  

A local authentication context to associate with the icon.

`controlSize`  

The size of the authentication view’s user interface element. Use one of the values in NSControl.ControlSize.

## Discussion

This initializer behaves like init(context:), except that it also allows you to specify a size for the view. If you don’t specify a size, the view uses the NSControl.ControlSize.regular size by default.

## See Also

### Controlling the size of a local authentication view

var controlSize: NSControl.ControlSize

The size of the local authentication view user interface element.

