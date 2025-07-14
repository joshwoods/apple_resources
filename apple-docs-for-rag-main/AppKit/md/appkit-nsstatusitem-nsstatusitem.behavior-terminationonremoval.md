

- AppKit
- NSStatusItem
- NSStatusItem.Behavior
-  terminationOnRemoval 

Type Property

# terminationOnRemoval

A status item that quits the application upon removal.

macOS 10.12+

``` source
static var terminationOnRemoval: NSStatusItem.Behavior { get }
```

## Discussion

A status item with this behavior quits the application if the user removes it from the menu bar. This behavior implicitly provides the same functionality as removalAllowed.

The terminationOnRemoval behavior is suitable for applications that display only a NSStatusItem and provide no other user interface.

## See Also

### Behaviors

static var removalAllowed: NSStatusItem.Behavior

A status item that allows interactive removal.

