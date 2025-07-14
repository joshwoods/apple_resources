

- CarPlay
- CPInterfaceController
-  prefersDarkUserInterfaceStyle 

Instance Property

# prefersDarkUserInterfaceStyle

A Boolean value that determines whether the system draws the user interface in Dark Mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var prefersDarkUserInterfaceStyle: Bool { get set }
```

## Discussion

To adopt the dark user interface style, set this value to true before you provide the root template or push any templates. The default value is false, which allows templates to change between light and dark styles.

## See Also

### Configuring the Interface Controller

var delegate: (any CPInterfaceControllerDelegate)?

An object that serves as the delegate to the interface controller.

protocol CPInterfaceControllerDelegate

The interface that an object implements to serve as a delegate to an interface controller.

func setRootTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Sets the root template of the navigation hierarchy.

