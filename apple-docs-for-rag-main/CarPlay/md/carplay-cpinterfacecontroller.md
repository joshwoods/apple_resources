

- CarPlay
-  CPInterfaceController 

Class

# CPInterfaceController

A controller that manages the templates for constructing a scene’s user interface.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPInterfaceController
```

## Overview

An interface controller manages one or more templates in the navigation hierarchy. You don’t create the interface controller. Instead, CarPlay creates one for you and passes it to the delegate of CPTemplateApplicationScene when the scene connects.

After receiving the controller, store a reference to it in your app. Then set the root template by calling the setRootTemplate(_:animated:completion:) method. To display another template in the navigation hierarchy, call pushTemplate(_:animated:completion:), and use popTemplate(animated:completion:) to remove the top-most template.

You also use the interface controller to display a single template modally. Call presentTemplate(_:animated:completion:) to display the modal template, and call dismissTemplate(animated:completion:) to dismiss it.

## Topics

### Configuring the Interface Controller

var delegate: (any CPInterfaceControllerDelegate)?

An object that serves as the delegate to the interface controller.

protocol CPInterfaceControllerDelegate

The interface that an object implements to serve as a delegate to an interface controller.

var prefersDarkUserInterfaceStyle: Bool

A Boolean value that determines whether the system draws the user interface in Dark Mode.

func setRootTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Sets the root template of the navigation hierarchy.

### Accessing the Trait Collection

var carTraitCollection: UITraitCollection

The trait collection of the vehicle’s primary screen.

### Accessing Templates

var rootTemplate: CPTemplate

The root template in the navigation hierarchy.

var topTemplate: CPTemplate?

The top-most template in the navigation hierarchy.

var templates: [CPTemplate]

The contents of the navigation hierarchy.

### Adding and Removing Templates

func pushTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Adds the specified template to the navigation hierarchy and displays it.

func popTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes the top-most template from the navigation hierarchy.

func popToRootTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes all of the templates from the navigation hierarchy except the root template.

func pop(to: CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes each template from the navigation hierarchy until the specified template becomes visible.

### Displaying Templates Modally

func presentTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Presents a template modally.

func dismissTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Dismisses a modal template.

var presentedTemplate: CPTemplate?

The interface controller’s current modal template.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accessing the Interface Controller

var interfaceController: CPInterfaceController

The controller that manages the scene’s user interface.

