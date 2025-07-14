

- AppKit
- NSStoryboardSegue
-  init(identifier:source:destination:performHandler:) 

Initializer

# init(identifier:source:destination:performHandler:)

Creates a storyboard segue and a block used when the segue is performed.

macOS 10.10+

``` source
convenience init(
    identifier: NSStoryboardSegue.Identifier,
    source sourceController: Any,
    destination destinationController: Any,
    performHandler: @escaping () -> Void
)
```

## Parameters 

`identifier`  

The unique identifier for the storyboard segue. See the identifier property.

`sourceController`  

The starting/containing view controller or window controller for the storyboard segue.

`destinationController`  

The ending/contained view controller or window controller for the storyboard segue.

`performHandler`  

A block of code that you provide, to be run each time the system calls the perform() method.

## Return Value

An initialized storyboard segue and code block, ready to be performed.

## Discussion

You can use this method to customize a storyboard segue in lieu of creating a subclass.

## See Also

### Customizing Storyboard Segue Initialization and Invocation

init(identifier: NSStoryboardSegue.Identifier, source: Any, destination: Any)

The designated initializer for a storyboard segue.

func perform()

Performs a visual transition from one controller to another.

