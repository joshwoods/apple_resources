

- Local Authentication Embedded UI
- LAAuthenticationView
-  init(context:) 

Initializer

# init(context:)

Creates a new authentication icon that reflects the current authentication state.

macOS 12.0+

``` source
@MainActor
init(context: LAContext)
```

## Parameters 

`context`  

A local authentication context to associate with the icon.

## Discussion

Use this initializer to create a local authentication view and connect it to a particular local authentication context. You typically do this in the doc://com.apple.documentation/documentation/appkit/nsviewcontroller/1434405-loadview method of an NSViewController subclass. You then add this view as a subview — along with any text, imagery, and interactive elements that you need — to create a custom authentication interface. When your interface appears, call the LAContext instance’s evaluatePolicy(_:localizedReason:reply:) method to begin the authentication process.

## See Also

### Creating a local authentication view

var context: LAContext

The local authentication context associated with the authentication view.

