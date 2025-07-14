

- TVMLKit
-  TVApplicationController Deprecated

Class

# TVApplicationController

An object that bridges the UI, navigation stack, storage, and event handling from JavaScript.

tvOS 9.0–18.0Deprecated

``` source
class TVApplicationController
```

Deprecated

Please use SwiftUI or UIKit

## Mentioned in 

Creating TVML Elements

## Overview

The `TVApplicationController` class establishes the JavaScript environment and provides a centralized point of control and coordination between the JavaScript environment and tvOS.

## Topics

### Creating a New App Controller

init(context: TVApplicationControllerContext, window: UIWindow?, delegate: (any TVApplicationControllerDelegate)?)

Initializes and returns an app controller.

### Controlling and Handling Events

func evaluate(inJavaScriptContext: (JSContext) -> Void, completion: ((Bool) -> Void)?)

Evaluates a block in the JavaScript execution queue.

func stop()

Ends the app life cycle.

### Getting the Delegate

var delegate: (any TVApplicationControllerDelegate)?

The delegate of the app controller object.

protocol TVApplicationControllerDelegate

A protocol used to observe and manage the different states of an application controller.

### Examining App Controller Properties

var context: TVApplicationControllerContext

The launch information for the application controller.

var navigationController: UINavigationController

The navigation controller that is bridged from JavaScript to tvOS.

var window: UIWindow?

A reference to the window supplied when the app controller was initialized.

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

### JavaScript Environment

Implementing a Hybrid TV App with TVMLKit

Display content options with document view controllers and fetch and populate content with TVMLKit JS.

class TVApplicationControllerContext

Launch information provided to the TV application controller.

Deprecated

