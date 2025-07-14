

- CarPlay
-  CPInterfaceControllerDelegate 

Protocol

# CPInterfaceControllerDelegate

The interface that an object implements to serve as a delegate to an interface controller.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
protocol CPInterfaceControllerDelegate : NSObjectProtocol
```

## Topics

### Handling Display Events

func templateWillAppear(CPTemplate, animated: Bool)

Tells the delegate that the template will appear onscreen.

func templateDidAppear(CPTemplate, animated: Bool)

Tells the delegate that the template did appear onscreen.

func templateWillDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template will disappear from the screen.

func templateDidDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template did disappear from the screen.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring the Interface Controller

var delegate: (any CPInterfaceControllerDelegate)?

An object that serves as the delegate to the interface controller.

var prefersDarkUserInterfaceStyle: Bool

A Boolean value that determines whether the system draws the user interface in Dark Mode.

func setRootTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Sets the root template of the navigation hierarchy.

