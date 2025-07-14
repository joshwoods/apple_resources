

- AppKit
- NSStoryboardSegue
-  init(identifier:source:destination:) 

Initializer

# init(identifier:source:destination:)

The designated initializer for a storyboard segue.

macOS 10.10+

``` source
init(
    identifier: NSStoryboardSegue.Identifier,
    source sourceController: Any,
    destination destinationController: Any
)
```

## Parameters 

`identifier`  

The unique identifier for the storyboard segue. See the identifier property.

`sourceController`  

The starting/containing view controller or window controller for the storyboard segue.

`destinationController`  

The ending/contained view controller or window controller for the storyboard segue.

## Return Value

An initialized storyboard segue, ready to be performed.

## Discussion

When a segue begins, the system calls this method. To run code during segue initialization, implement a storyboard segue subclass and override this method.

Whenever this method is called, the system then calls the perform() method.

## See Also

### Customizing Storyboard Segue Initialization and Invocation

convenience init(identifier: NSStoryboardSegue.Identifier, source: Any, destination: Any, performHandler: () -> Void)

Creates a storyboard segue and a block used when the segue is performed.

func perform()

Performs a visual transition from one controller to another.

