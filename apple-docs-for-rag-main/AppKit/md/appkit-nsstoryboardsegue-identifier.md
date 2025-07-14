

- AppKit
- NSStoryboardSegue
-  identifier 

Instance Property

# identifier

An optional, unique identifier for the storyboard segue that you can specify using the Identity inspector in Interface Builder.

macOS 10.10+

``` source
var identifier: NSStoryboardSegue.Identifier? { get }
```

## Discussion

You use this property if you override the prepare(for:sender:) method of the NSSeguePerforming protocol.

## See Also

### Inspecting a Storyboard Segue

var sourceController: Any

The starting/containing view controller or window controller for the storyboard segue.

var destinationController: Any

The ending/contained view controller or window controller for the storyboard segue.

typealias Identifier

