

- AppKit
- NSStoryboardSegue
-  sourceController 

Instance Property

# sourceController

The starting/containing view controller or window controller for the storyboard segue.

macOS 10.10+

``` source
var sourceController: Any { get }
```

## Discussion

In your storyboard segue subclass, you can read this property to get the starting/containing view controller or window controller for the segue.

## See Also

### Inspecting a Storyboard Segue

var destinationController: Any

The ending/contained view controller or window controller for the storyboard segue.

var identifier: NSStoryboardSegue.Identifier?

An optional, unique identifier for the storyboard segue that you can specify using the Identity inspector in Interface Builder.

typealias Identifier

