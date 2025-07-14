

- AppKit
-  NSStoryboardSegue 

Class

# NSStoryboardSegue

A transition or containment relationship between two scenes in a storyboard.

macOS 10.10+

``` source
class NSStoryboardSegue
```

## Overview

In this context, a *scene* is a view controller or a window controller and a *storyboard* is an instance of the NSStoryboard class.

A storyboard segue has a procedural notion of being invoked, known in the API as being *performed*. You can take advantage of hooks into the segue performance process by way of the NSSeguePerforming protocol.

You do not create storyboard segue objects directly. Instead, the system creates them as needed as segues are invoked. To run code during initialization and performance of a segue, override the init(identifier:source:destination:) and perform() methods.

You can initiate a segue programmatically with the performSegue(withIdentifier:sender:) method of the NSSeguePerforming protocol. For example, you might do this to transition from a scene in one storyboard file to a scene in another.

## Topics

### Inspecting a Storyboard Segue

var sourceController: Any

The starting/containing view controller or window controller for the storyboard segue.

var destinationController: Any

The ending/contained view controller or window controller for the storyboard segue.

var identifier: NSStoryboardSegue.Identifier?

An optional, unique identifier for the storyboard segue that you can specify using the Identity inspector in Interface Builder.

typealias Identifier

### Customizing Storyboard Segue Initialization and Invocation

convenience init(identifier: NSStoryboardSegue.Identifier, source: Any, destination: Any, performHandler: () -> Void)

Creates a storyboard segue and a block used when the segue is performed.

init(identifier: NSStoryboardSegue.Identifier, source: Any, destination: Any)

The designated initializer for a storyboard segue.

func perform()

Performs a visual transition from one controller to another.

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

### Storyboard

class NSStoryboard

An encapsulation of the design-time view controller and window controller graph represented in an Interface Builder storyboard resource file.

protocol NSSeguePerforming

A set of methods that support the mediation of a custom segue.

