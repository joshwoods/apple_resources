

- CarPlay
- CPInterfaceController
-  delegate 

Instance Property

# delegate

An object that serves as the delegate to the interface controller.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
weak var delegate: (any CPInterfaceControllerDelegate)? { get set }
```

## See Also

### Configuring the Interface Controller

protocol CPInterfaceControllerDelegate

The interface that an object implements to serve as a delegate to an interface controller.

var prefersDarkUserInterfaceStyle: Bool

A Boolean value that determines whether the system draws the user interface in Dark Mode.

func setRootTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Sets the root template of the navigation hierarchy.

