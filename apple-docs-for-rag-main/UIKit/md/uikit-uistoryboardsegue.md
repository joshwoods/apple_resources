

- UIKit
-  UIStoryboardSegue 

Class

# UIStoryboardSegue

An object that prepares for and performs the visual transition between two view controllers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class UIStoryboardSegue
```

## Mentioned in 

Customizing the behavior of segue-based presentations

Dismissing a view controller with an unwind segue

## Overview

The UIStoryboardSegue class supports the standard visual transitions available in UIKit. You can also subclass to define custom transitions between the view controllers in your storyboard file.

Segue objects contain information about the view controllers involved in a transition. When a segue is triggered, but before the visual transition occurs, the storyboard runtime calls the current view controller’s prepare(for:sender:) method so that it can pass any needed data to the view controller that’s about to be displayed.

You don’t create segue objects directly. Instead, the storyboard runtime creates them when it must perform a segue between two view controllers. You can still initiate a segue programmatically using the performSegue(withIdentifier:sender:) method of UIViewController if you want. You might do so to initiate a segue from a source that was added programmatically and therefore not available in Interface Builder.

### Subclassing notes

You can subclass UIStoryboardSegue in situations where you want to provide a custom transition between view controllers in your application. To use your custom segue, create a segue line between the appropriate view controllers in Interface Builder and set its type to Custom in the inspector; you must also specify the class name of the segue to use in the inspector.

When the storyboard runtime detects a custom segue, it creates a new instance of your class, configures it with the view controller objects, asks the view controller source to prepare for the segue, and then performs the segue.

#### Methods to override

For custom segues, the main method you need to override is the perform() method. The storyboard runtime calls this method when it’s time to perform the visual transition from the view controller in source to the view controller in destination. If you need to initialize any variables in your custom segue subclass, you can also override the init(identifier:source:destination:) method and initialize them in your custom implementation.

#### Alternatives to subclassing

If your segue doesn’t need to store additional information or provide anything other than a perform() method, consider using the init(identifier:source:destination:performHandler:) method instead.

## Topics

### Initializing a storyboard segue

init(identifier: String?, source: UIViewController, destination: UIViewController)

Initializes and returns a storyboard segue object for use in performing a segue.

### Accessing the segue attributes

var source: UIViewController

The source view controller for the segue.

var destination: UIViewController

The destination view controller for the segue.

var identifier: String?

The identifier for the segue object.

### Performing the segue

func perform()

Performs the visual transition for the segue.

### Creating a custom segue

convenience init(identifier: String?, source: UIViewController, destination: UIViewController, performHandler: () -> Void)

Creates a segue that calls a block to perform the segue transition.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIStoryboardPopoverSegue

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Storyboards

Customizing the behavior of segue-based presentations

Pass data between view controllers during a segue, and programmatically control when segues occur.

Dismissing a view controller with an unwind segue

Configure an unwind segue in your storyboard file that dynamically chooses the most appropriate view controller to display next.

class UIStoryboard

An encapsulation of the design-time view controller graph represented in an Interface Builder storyboard resource file.

class UIStoryboardUnwindSegueSource

An encapsulation of information about an unwind segue.

