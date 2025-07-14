

- AppKit
- NSStoryboardSegue
-  destinationController 

Instance Property

# destinationController

The ending/contained view controller or window controller for the storyboard segue.

macOS 10.10+

``` source
var destinationController: Any { get }
```

## Discussion

In your storyboard segue subclass, you can read this property to get the ending/contained view controller or window controller for the segue. This property is essential if you override the prepare(for:sender:) method of the NSSeguePerforming protocol, to let you pass configuration data to the ending/contained controller.

## See Also

### Inspecting a Storyboard Segue

var sourceController: Any

The starting/containing view controller or window controller for the storyboard segue.

var identifier: NSStoryboardSegue.Identifier?

An optional, unique identifier for the storyboard segue that you can specify using the Identity inspector in Interface Builder.

typealias Identifier

