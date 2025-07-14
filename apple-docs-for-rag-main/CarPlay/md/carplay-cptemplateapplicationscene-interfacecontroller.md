

- CarPlay
- CPTemplateApplicationScene
-  interfaceController 

Instance Property

# interfaceController

The controller that manages the scene’s user interface.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var interfaceController: CPInterfaceController { get }
```

## Discussion

Use this property to access the interface controller CarPlay creates when the scene connects, which you then use to manage your templates.

## See Also

### Accessing the Interface Controller

class CPInterfaceController

A controller that manages the templates for constructing a scene’s user interface.

